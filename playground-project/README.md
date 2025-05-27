
# Application
This repository contain the demo Java application with unit tests

# Build
It has the docker file to build the image

# CI
It has the Jenkins file to do the orchestration of running the maven build , unit tests, docker build and push to Docker hub and then deploy on k8

# Deploy
It will deploy to a kubernetes cluster GKE using a service account having k8 Deployment role, and using the Jenkins plugin, by getting the deployment manifest in manifest.yaml. The deployment will pull the image from Docker hub using secrets in dockerconfigjson
