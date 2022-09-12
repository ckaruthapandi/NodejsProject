pipeline {
  agent any
  environment{
    GIT_COMMIT = getcommitid()
  }
 
  stages {
  
    stage('Node js app clone') {
      steps {
        git branch: 'main', url: 'https://github.com/ckaruthapandi/NodejsProject.git'
        script {
          env.GIT_COMMIT_MSG = sh (script: 'git log -1 --pretty=%B ${GIT_COMMIT}', returnStdout: true).trim()
        }
      }
    } 
    stage('Docker image build ') {
      steps {
        sh 'docker build -t aatmaaniproject .'
      }
    }
    stage('Pushing to ECR') {
      steps {  
        script {
                sh 'aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 581962848636.dkr.ecr.us-east-1.amazonaws.com'
                sh 'docker tag aatmaaniproject:latest 581962848636.dkr.ecr.us-east-1.amazonaws.com/aatmaaniproject: ${DRONE_COMMIT_SHA:0:8}'
                sh 'docker tag aatmaaniproject:latest 581962848636.dkr.ecr.us-east-1.amazonaws.com/aatmaaniproject:devlatest'
                sh 'docker push 581962848636.dkr.ecr.us-east-1.amazonaws.com/aatmaaniproject: ${DRONE_COMMIT_SHA:0:8}'
                sh 'docker push 581962848636.dkr.ecr.us-east-1.amazonaws.com/aatmaaniproject:devlatest'
        }
      }
    }
  }
post 
  {
      always
      {
          slackSend channel: 'kp-devops', message: "pipeline status -${currentBuild.currentResult}"
        }
   }
}
 def getcommitid(){
    def tag = sh script: 'git rev-parse HEAD', returnStdout: true
    return tag
 }
