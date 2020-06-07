# AKASH TOOLS

## Ansible 
### Validator / sentry node Installation playbook

```sh
ansible-playbook -i hosts.ini install.yml -e "NODE_GROUP=sentry" -t sentry --ask-become-pass ## to run a sentry node installation
ansible-playbook -i hosts.ini install.yml -e "NODE_GROUP=validator" -t validator --ask-become-pass ## to run a valiator node installation
ansible-playbook -i hosts.ini new-user.yml -e "NODE_GROUP=validator" ## to create a user with homepage and add your pubkey in ~/.ssh
```

``` -e "NODE_GROUP=validators" ``` means the correct host group to deploy on\
``` -t sentry ``` means to deploy sentry on selected host group\
``` -t validator ``` means to deploy validator on selected host group

