The project uses ansible to deploy the Task1 https://github.com/shubarna-tech/HAZESOFT-T1.git to a Ansible Host machine.
This requires host and master node ssh connections and configurations over ansible host files.

Install Ansible: https://docs.ansible.com/ansible/latest/installation_guide/index.html

## Check Master and Node connection with command:
ansible all -m ping -u ubuntu

## To run the ansible playbook use the command:
ansible-playbook -i hostMachine_ip, -u ubuntu -K deploy.yml

## check output over host machine with curl command
curl http://localhost:9000/site/index.html

Please refer to screenshots folder for additional help.