# environment-setup-ansible

My environment setup using ansible

Currently installing

- basic
  - stow
  - kitty
  - htop
  - starship(terminal)
- asdf
  - helm
  - kubectl
  - golang
  - k9s
  - kubectl
  - rust
  - terraform
  - nodejs
  - lazygit
- neovim

## Pre-requirements

- [Dotfiles](https://github.com/uelei/dotfiles) repo to be used (using stow)
- Change all variables on vars/vars.yml
  - for macos group is staff on linux is the same as the user

### For MacOs

```bash
xcode-select --install
# install Brew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# install ansible using brew
brew install ansible
```

### Install Pre-requirements

```bash
sudo pip install ansible  # linux only
ansible-galaxy install -r requirements.yml
```

## To run

The following command is going to ask you BECOME_PASSWORD, it is your password to become sudo

```bash
ansible-playbook main.yml -K
```

## To install latest packages for asdf

Set vars/vars.yml the variable `add_asdf_latest_packages` to true
