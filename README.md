# Terralogic-Task
Automating deploying and cleaning up Kubernetes microservices using Ansible Playbooks.

## Structure of files and roles in tree formate
etc/
|__ansible/
    |__ansible.cfg
    |__cleanup.yaml
    |__deploy.yaml
    |__group_vars/
        |__all.yaml
    |__inventory
    |__hosts
    |__roles/
        |__service-a/
          |__files/
              |__deployment.yaml
              |__service.yaml
          |__tasks/
              |__deploy.yaml
              |__cleanup.yaml
        |__service-b/
            |__files/
                |__deployment.yaml
                |__service.yaml
            |__tasks/
                |__deploy.yaml
                |__cleanup.yaml

### Showing result after running playbook for deploying
![image](https://github.com/user-attachments/assets/1fe96322-cf0e-48b6-b5cb-edee507d5cd7)

### showing pods, deployments & services created and running on k8s master
![image](https://github.com/user-attachments/assets/a5f69f59-29b1-4f20-a8cb-b9ca98ebca0c)

### Showing result after running playbook for cleaning up
![image](https://github.com/user-attachments/assets/9a01046f-8e82-4ad0-8a8d-d776e6ccfc88)

### showing pods, deployments & services deleted from k8s master
![image](https://github.com/user-attachments/assets/2a3767b9-4ae0-47b0-82ca-f4f61f371133)
