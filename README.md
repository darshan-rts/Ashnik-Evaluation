## Kubernetes Cluster Setup
1. To setup K8s cluster using minikube in mac os follow the following steps.
   
    brew install minikube
   
3. If minikube is already installed in your mac please follow the following Steps.
   
    brew unlink minikube
   
    brew link --overwrite minikube
   
5. Start MiniKube Cluster.
   
   minikube start
   
## Nginx Ingress Setup:  

1. Install helm in macos.
   
   brew install helm chart.
   
3. Install Nginx Controller version 1.3.1 in ingress-controller namespace using following command. This helm command with install nginx-ingress controller as daemon set with "nginx-ingress" as a release name

   kubectl create namespace ingress-controller  

   helm install nginx-ingress oci://ghcr.io/nginxinc/charts/nginx-ingress --version 1.3.1 -n ingress-controller

5. Install ingress.yaml in ashnik  namespace file using the following command.
   
  kubectl create namespace ashnik
 
  kubectl apply -n ashnik-test -f ingress.yaml 


 
