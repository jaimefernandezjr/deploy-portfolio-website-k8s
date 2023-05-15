# deploy-portfolio-website-k8s
a deployment of my porfolio website using Kubernetes minikube

## What is happening in this project?
1. Deploy in Kubernetes cluster using a deployment manifest file that obtains the portfolio-website's image from dockerhub from https://github.com/jaimefernandezjr/cicd-dockerize-app

## How to run this project
1. Install Minikube. Make sure Docker Desktop is running.
2. Start minikube using ```minikube start```
3. Go to tourist-k8s folder and run the command ```kubectl apply -f v1.yml```
4. Using ```kubectl get pods```, wait until all pods are running
5. run ```kubectl get service``` and get the service name of the application
6. run ```minikube service <service-name>``` to access the website on your favorite browser

## Extras
1. The website is using a load balancer, meaning that different pods are being utilize when the website is refreshed
