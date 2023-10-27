# eks-task
Create the K8s EKS,further you have to do the deployment of Nginx application

Create an EKS Cluster:

eksctl create cluster --name my-eks-cluster --region us-east-1

Configure kubectl:
After creating the EKS cluster, configure kubectl to use it

aws eks --region us-east-1 update-kubeconfig --name my-eks-cluster

Create a Deployment

kubectl apply -f nginx-deployment.yaml

Expose the Deployment

kubectl apply -f nginx-service.yaml


Access the Nginx Application

kubectl get svc nginx-service

![Screenshot (273)](https://github.com/cloudmoh/eks-task/assets/126796948/468761a7-ea7a-4122-a110-122da40d32c9)
![Screenshot (274)](https://github.com/cloudmoh/eks-task/assets/126796948/33dee2d8-b89c-448f-aa74-01dc23cb0546)


