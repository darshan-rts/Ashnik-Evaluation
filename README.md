## Kubernetes Cluster Setup
1. To setup K8s cluster using minikube in mac os follow the following steps.
   
    brew install minikube
2. If minikube is already installed in your mac please follow the following Steps.
   
    brew unlink minikube
   
    brew link --overwrite minikube

## Nginx Ingress Setup:  
1. Install helm in macos.
   
   brew install helm chart.
   
3. Install Nginx Controller using following command.
   
   helm install my-release oci://ghcr.io/nginxinc/charts/nginx-ingress --version 1.3.1


 
