# ToyTrendz
A Toy Retail company ToyTrex has it retail application deployed as 3-tier application - Web App(UI), Web API(middle layer) and Database as Azure SQL.
The user load started increasing multiple fold every month and complex programs getting implemented, the application started performing poorly.
As a result, company decided to re-architect the middle layer as microservices using Azure Kubernetes Services.
The new architecture has below design decisions.

1) The middle layer should be implemented as Microservices using Azure AKS
2) The middle layer API should be deployed as containerized application images
3) The container images will use Azure Container Repository (ACR) as the private image repository
4) The CI/CD pipelines for microservices should be implemented using Azure DevOps services.
5) The Azure DevOps should be able to access ACR and download the container images for microservices deployment
6) The image should be deployed as templates such as <image_name>:<build_id>
