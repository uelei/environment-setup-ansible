# environment-setup-ansible  
My environment setup using ansible

## Pre-requirements  
- [Dotfiles](https://github.com/uelei/dotfiles) repo to be used (using stow)  
- Change all variables on vars/vars.yml

## To run  
 
The following command is going to ask you BECOME_PASSWORD, it is your password to become sudo
```bash
ansible-playbook main.yml -K 
```
