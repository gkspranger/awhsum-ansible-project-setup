# awhsum-ansible-project-setup
wut an ideal ansible project setup could look like

if you use the {{ inventory_dir }} variable to include custom vars found in ./inventories/vars/* -- it means your inventory would HAVE to be a child of the inventories DIR ..
this isn't so bad because you really should have a dynamic inventory that discovers nodes vs static files .. but hey, we all have to start somewhere

```bash
# ALL commands executed in the same dir as the ansible.cfg

# example kicking the provision playbook
ansible-playbook -i inventories/localhost playbooks/provision/example.yml

# example kicking the configure playbook
ansible-playbook -i inventories/localhost playbooks/configure/example.yml

# example kicking the deploy playbook
ansible-playbook -i inventories/localhost playbooks/deploy/example.yml
```
