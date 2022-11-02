# Project requirments:

 <img  src="Requirments.jfif">

# ITI DevOps Track Final Project

Using Docker, terrafrom , GCP , Helm , Kubernetes and jenkins to Deploy a nodejs web application on GKE by CI/CD Pipeline. 

### [ Infrastructure Repository ](https://https://github.com/karimomar71/Nodejs_App)
- apply infrastructure with [Terraform ](https://github.com/karimomar71/Nodejs_App/tree/main/terraform) in GCp 
- Instaling jenkins in cluster with  [helm](https://github.com/karimomar71/Final-Project-App/blob/main/k8s/README.md)  

### Steps are as following:
- dockerize NodeJS application
- configure Credentials in Jenkins
- create CI pipeline with Jenkins
- Create CD pipline with  Jenkins
- Create a webhook to apply dynamic changes

# dockerize my app 
- [ Dockerfile ](https://github.com/karimomar71/Final-Project-App/blob/main/Dockerfile) 

# Create Jenkins Pipelines

 <img  src="Jenkins/Pipeline.jfif">

# Add Credentials in Jenkins
 - github Credentials
 - dockerhub Credentials
 - serviceaccount Credentials

# create Continuous Integration CI pipline :

  -  pull code from github 
  -  build node-app image using docker and buildah to build your image
  -  push this image to dockerhub
  -  trigger CD pipline to run
  
# create CD Pipline
  - apply deployment application in K8s
