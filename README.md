### Kubernetes Cluster Setup

##### 1. To setup K8s cluster using minikube in mac os follow the following steps.
      
      brew install minikube
   
##### 2. If minikube is already installed in your mac please follow the following Steps.
      
      brew unlink minikube
      brew link --overwrite minikube
   
##### 3. Start MiniKube Cluster.

      minikube start
   
### Nginx Ingress Setup:  

##### 1. Install helm in macos.

      brew install helm
   
##### 2. Install Nginx Controller version 1.3.1 in ingress-controller namespace using following command. This helm command with install nginx-ingress controller as daemon set with "nginx-ingress" as a release name

      kubectl create namespace ingress-controller  
      helm install nginx-ingress oci://ghcr.io/nginxinc/charts/nginx-ingress --version 1.3.1 -n ingress-controller

##### 3. Install ingress.yaml in ashnik namespace using the following command.
   
      kubectl create namespace ashnik-evaluation
      kubectl apply -f ingress.yaml 
      
### Sample Application Deployment

##### Run hello-world manifest file to install application.

      kubectl apply -f hello-world.yaml
