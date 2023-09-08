![alt text](ecs.logo.JPG)
* This repository contains ansible roles to apply to hardened RHEL8 ec2 post deployment. For any additional details or inquiries, please contact us at csargent-ctr@ecstech.com.

# Deploy from GitHub
1. ssh or console to EC2
2. sudo -i 
3. cd /root
4. git clone https://github.com/ChristopherSargent/ecs_rhel8_ansible_base.git
5. cd ecs_rhel8_ansible_base
6. vim rhel8_ansible_base.yml
* include_role docker for version 23.0.6 or docker-ece for 20.10.24
```
# Ansible base roles for PreStaging Christopher Sargent 09062023
---
  - name: Install Docker-CE
    hosts: all
    gather_facts: true
    become_user: root
    tasks:
      - include_role:
          name: docker
```
7. ansible-playbook -i "localhost," -c local rhel8_ansible_base.yml -vvv
