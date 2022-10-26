# environment-setup-ansible  
My environment setup using ansible

Currently installing

- basic
  - stow
  - kitty
  - htop
  - starship(terminal)
- pyenv
  - pipx
  - poetry
- gvm
  - go 1.7.1
  - go 1.19.2
- nvm 
  - node lts
- rust
  - bat
- tfenv
- kubectl
- neovim


## Pre-requirements  
- [Dotfiles](https://github.com/uelei/dotfiles) repo to be used (using stow)  
- Change all variables on vars/vars.yml
    - for macos group is staff on linux is the same as the user

## For MacOs

```bash
sudo easy_install pip
sudo pip install ansible
ansible-galaxy collection install community.general
```

## To run  
 
The following command is going to ask you BECOME_PASSWORD, it is your password to become sudo
```bash
ansible-playbook main.yml -K 
```
