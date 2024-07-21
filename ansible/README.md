 ### Ansible Automation

##### 1. Validate whether k8s module is present.
 
    ansible-galaxy collection list | grep kubernetes  

##### 2. Run following command to install nginx controller in ingress-controller namespace.

    ansible-playbook ingress-controller-playbook.yaml
      
##### 3.  Run following command to deploy hello world app.

    ansible-playbook helloworld-playbook.yaml
      
### Security with TLS/SSL

#### Prerquisite.

#### Install Nginx Controller mentioned in step 2 of Ansible Automation.


##### To generate certificate and enable it for nginx ingress run the following command 

    ansible-playbook enable-ssl-ingress-playbook.yaml

     


