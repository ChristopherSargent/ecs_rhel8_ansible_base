![alt text](ecs.logo.JPG)
* This repository contains ansible roles to apply to hardened RHEL8 ec2 post deployment. For any additional details or inquiries, please contact us at csargent-ctr@ecstech.com.

# Configure GIT for Test ansible project to show Docker version
1. ssh or console to EC2
2. sudo -i 
3. cd /root
4. git clone https://github.com/ChristopherSargent/ecs_rhel8_ansible_base.git
5. cd cd ecs_rhel8_ansible_base
6. ansible-playbook -i "localhost," -c local rhel8_ansible_base.yml -vvv
