# awhsum-ansible-project-setup
wut an ideal ansible project setup could look like

```bash
# ALL commands executed in the same dir as the ansible.cfg

# example kicking the provision playbook
ansible-playbook -i inventories/localhost playbooks/provision/example.yml

# example kicking the configure playbook
ansible-playbook -i inventories/localhost playbooks/configure/example.yml

# example kicking the deploy playbook
ansible-playbook -i inventories/localhost playbooks/deploy/example.yml
```
