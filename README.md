# Nodejs Project overview 
- A simple Express-based app to test Node.js support. devops framework for building CI/CD pipeline in aws.
- A pipeline helps automate steps software deployment process, such as initiating automatic builds and then deploying to EKS cluster. used github repository, a service that builds in jenkins, tested in EKS test  enviroment , and deploys code every time there is a code change, based on the EKS name space. Use Docker to orchestrate each step in your release process. used Jenkins to completed software deployment pipeline. created a very simple pipeline that pulls code from a source repository and automatically deploys EKS cluster.
- 
`<Github repo>` https://github.com/ckaruthapandi/NodejsProject
`<Github repo>` https://github.com/ckaruthapandi/devops

### Diagram
![](https://raw.githubusercontent.com/ckaruthapandi/diagram/main/nodejaapp.png)
# Phase 1
### Continuous Integration
Continuous integration (CI) is the software engineering practice that requires frequent commits to a shared repository.
people would work on feature branches for weeks or months and then try to merge this branch to a main branch. Think about all that could go wrong during such merge — merge conflicts and failing tests, just to mention a few.

Continuous integration tries to prevent all of these by encouraging small and frequent code updates. When a code is committed to a repository, it can be built and tested against setup workflows to ensure that the code does not introduce any errors.

![](https://raw.githubusercontent.com/ckaruthapandi/diagram/main/CI.drawio.png)
# Phase 2
### Continuous Deployment
Continuous deployment means code changes are automatically deployed/released to a testing or production environment as soon as they are merged. This is often interchanged with continuous delivery and that’s because they are very similar.

![](https://raw.githubusercontent.com/ckaruthapandi/diagram/main/CD.png)
# Phase 3
### Continuous Monitoring
Continuous monitoring is the process and technology used to detect compliance and risk issues associated with an organization's financial and operational environment. The financial and operational environment consists of people, processes, and systems working together to support efficient and effective operations.

![](https://raw.githubusercontent.com/ckaruthapandi/diagram/main/monitor.png)
## AWS service 
- EC2
- ECR
- EKS
- Load Balancer
## Tools
- Git
- Github
- Jenkins
- Jenkins
- Kubernete
- Terraform
- slack
- Docker
- helm charts
- node exporter
- fluent bit
- promotheus
- elastic search 
- grafana
- kibana

## Git
GIT plays a vital role in code management that the collaborators deliver to the shared repository (data space where you save your files). The code is now extracted to perform continuous integration, created, and then tested on the server, then deployed in the products.
## GitHub
GitHub is an Internet hosting service for software development and version control using Git. It provides the distributed version control of Git plus access control, bug tracking, software feature requests, task management, continuous integration for every project.
## Jenkins
Jenkins offers a simple way to set up a continuous integration or continuous delivery (CI/CD) environment for almost any combination of languages and source code repositories using pipelines, as well as automating other routine development tasks
## Kubernetes
Kubernetes, also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications.
## Terraform
Terraform is an infrastructure as code tool that lets you define both cloud and on-prem resources in human-readable configuration files that you can version, reuse, and share. You can then use a consistent workflow to provision and manage all of your infrastructure throughout its lifecycle. Terraform can manage low-level components like compute, storage, and networking resources, as well as high-level components like DNS entries and SaaS features.
## slack
Slack is a messaging app for business that connects people to the information that they need. By bringing people together to work as one unified team, Slack transforms the way that organisations communicate.
## Docker
Slack is a messaging app for business that connects people to the information that they need. By bringing people together to work as one unified team, Slack transforms the way that organisations communicate.
## Helm Charts
Helm helps you manage Kubernetes applications — Helm Charts help you define, install, and upgrade even the most complex Kubernetes application.
Charts are easy to create, version, share, and publish — so start using Helm and stop the copy-and-paste.
## Fluent Bit
Fluent Bit allows to collect log events or metrics from different sources, process them and deliver them to different backends such as Fluentd, Elasticsearch, Splunk, DataDog, Kafka, New Relic, Azure services, AWS services, Google services, NATS, InfluxDB or any custom HTTP end-point.
## Prometheus
Prometheus, a Cloud Native Computing Foundation project, is a systems and service monitoring system. It collects metrics from configured targets at given intervals, evaluates rule expressions, displays the results, and can trigger alerts when specified conditions are observed.
## Elasticsearch
Elasticsearch is a distributed, free and open search and analytics engine for all types of data, including textual, numerical, geospatial, structured, and unstructured. Known for its simple REST APIs, distributed nature, speed, and scalability, Elasticsearch is the central component of the Elastic Stack, a set of free and open tools for data ingestion, enrichment, storage, analysis, and visualization. Commonly referred to as the ELK Stack (after Elasticsearch, Logstash, and Kibana), the Elastic Stack now includes a rich collection of lightweight shipping agents known as Beats for sending data to Elasticsearch.
## Grafana
Grafana is a multi-platform open source analytics and interactive visualization web application. It provides charts, graphs, and alerts for the web when connected to supported data sources.
## Kibana
Kibana is a source-available data visualization dashboard software for Elasticsearch, whose free and open source successor in OpenSearch is OpenSearch Dashboards.

