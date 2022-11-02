# Final Project

using Docker, terrafrom , GCP , Helm , Kubernetes and jenkins 

Deploy a nodejs web application on GKE by CI/CD Pipeline. 

#
### First Part: [ Infrastructure Repository ](https://github.com/mostafaashour99/Final-project-Infra)
- apply infrastructure with [Terraform ](https://github.com/mostafaashour99/Final-project-Infra/tree/main/terraform) in GCp 
- Instaling jenkins in cluster with  [helm](https://github.com/mostafaashour99/Final-project-Infra/tree/main/jenkins)  
### second part:
- dockerize python application
- configure Credentials in Jenkins
- create CI pipeline with Jenkins
- Create CD pipline with  Jenkins

# dockerize my app 
- [ Dockerfile ](https://github.com/mostafaashour99/Final-Project-app/blob/main/Dockerfile) 

# Add Credentials in Jenkins
 - github Credentials
 - dockerhub Credentials
 - serviceaccount Credentials

# create Continuous Integration CI pipline :
  -  pull code from github 
  -  build py-app image you can use (docker - buildah - kaniko - or anything else) to build your image
  -  push this image to dockerhub
  -  trigger CD pipline to run
  
# create CD Pipline
  - apply deployment application in K8s