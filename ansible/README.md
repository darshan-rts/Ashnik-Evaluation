 ### Ansible Automation

##### 1. Validate whether k8s module is present.
 
    ansible-galaxy collection list | grep kubernetes  

##### 2. Run following command to install nginx controller in ingress-controller namespace.

    ansible-playbook ingress-controller-playbook.yaml
      
##### 3.  Run following command to deploy hello world app.

    ansible-playbook helloworld-playbook.yaml
      
### Security with TLS/SSL

##### 1. Create selfsigned certificate using following Playbook.

    ansible-playbook openssl-playbook.yaml

##### 2. Create secret
     


