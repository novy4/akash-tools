# AKASH TOOLS

## Ansible 
### Validator / sentry node Installation playbook

```sh
ansible-playbook -i hosts.ini install.yml -e "NODE_GROUP=" -t sentry --ask-become-pass ## to run a sentry node installation\
ansible-playbook -i hosts.ini install.yml -e "NODE_GROUP=" -t validator --ask-become-pass ## to run a valiator node installation
```

``` -e "NODE_GROUP=validators" ``` means the correct host group to deploy on\
``` -t sentry ``` means to deploy sentry on selected host group\
``` -t validator ``` means to deploy validator on selected host group\

