# k8s-FastAPI-project
Kubernetes (or K8s) is an open source container orchestrator maintained by the Cloud Native Computing Foundation (CNCF). Thanks to its highly advanced features and large number of contributors, Kubernetes has become a de facto standard over time, supplanting Mesos and Docker Swarm, for example. As a DevOps engineer, getting to grips with Kubernetes and implementing it is essential.
------------------------------------------------------------------------------------------------
# Deploying a secure application
Context and objective:
 Example for deploying new microservices that will enable the registration and counting of users present on this platform. To do this, there are  2 microservices to deploy:
 
-  a service that will deploy the  FastAPI application.  - a second service that will deploy your PostgresSQL database

   ---------------------------------------------------------------------

For the successful completion of your assignment, we have prepared a roadmap for you:

Define the appropriate Kubernetes objects for optimal deployment of microservices, you have the choice for the type of object to use.

Write the Dockerfile for the microservice FastAPI. The application is available on the following repository: kubernetes-devops-project.git.

Base yourself on the docker-compose.yaml file in order to understand the architecture to be deployed.

You will create your subdomain at https://cloudns.net and create a registration for your website.

You will use Rancher's default storage class (StorageClass) to manage your storage for your application. Your storage volume will have 10 Gb of storage and should allow multiple Pods to write to it.

You will define 3 replicas of your application when it is deployed.

You will also need to prepare a backup plan for your cluster using the K3s client.

All tasks will need to be set up in this way:

Deployment using Kubernetes' standard YAML files, to deploy them you will use the Namespace standard.
Deliverables:

To validate the exercise you will need to send in Zip format:

A YAML-STANTARD directory with all the configurations.

The log files for your various microservices (FastAPI, PostgreSQL).

A backup file of your ETCD database once all the configurations set up have been deployed.

A few tips to get you started:

Each microservice will need to be exposed via a service so that other microservices can connect to a specific port.

The only Pod with which we will be able to connect via ingress is that of the FastAPI application.

Be sure to choose your objects according to the type of application (Stateful, Stateless) or according to confidentiality (ConfigMap, Secret)

To populate your database you can do this on the /docs route of your micro-service FastAPI.

For the list of users, the route is /users.

For the count of all users on the platform, the route is /users/count.









