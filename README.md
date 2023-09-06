
# Configure GIT for Test ansible project to show Docker version
1. ssh christopher.sargent@ps-awx01-terraform-nlb-71fdcacfa59d60d0.elb.us-gov-west-1.amazonaws.com
2. git config --global user.name "Chris Sargent"
3. git config --global user.email "chris.sargent-CTR@ecstech.com"
4. git clone https://bitbucket.cdmdashboard.com/scm/dbops/ansible_rhel8_verify.git
5. cd /home/christopher.sargent/ansible_rhel8_verify/ansible/ansible_rhel8_verify
6. sudo ansible-playbook -i "localhost," -c local ansible_rhel8_verify.yml -vvv
