# bootcamp_devops-ansible_mini-projet
Deploy Apache with docker by creating Ansible rule webapp

## Security notes

### encrypt with ansible-vault

To encrypt some file run and set the vault password:
> ansible-vault encrypt files/secrets/credentials.yml

Run this command to execute your playbook now:
> ansible-playbook -i inventory.yml deploy.yml --ask-vault-pass

### Ansible ssh key

To generate ssh key and copy it to the remote host, run these commands below:
> ssh-keygen -t rsa

> ssh-copy-id admin@[ip_address]