# kubenetes-apache-webapp
Create a EKS Cluster using eksctl

Run the following command to create an EKS cluster named playground-cluster with 3 nodes in the us-west-2 region
command: eksctl create cluster --name playground-cluster --region us-west-2 --nodes 3 --nodes-min 1 --nodes-max 4 --managed
Eks setup with pods which consists of a container running the image fotso2024/fotso_apache_image:v1.0.1 
Command: kubectl apply -f To apply the manifest file located
create a deployment for our application with 2 replica of our pod
Command: kubectl apply -f deployment.yml
Command:kubectl get deployments
Command:kubectl get pods
Command:kubectl describe deployment apache-deployment
Create a load balancer service to expose our application on port 80
command:kubectl apply -f loadbalancer-service.yml
command:kubectl get services
external IP:af1facd74b5b54aeca47c73b04c5e2a4-476477138.us-west-2.elb.amazonaws.com 

