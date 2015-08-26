Vagrant-Ansible-CentOS
===============
This is Ansible playbook to provision a CentOS box suitable for production on a local Vagrant environment.

## Stack
* CentOS 6.6
* Git 2.5.0
* dotfiles (install my dotfiles based on https://github.com/shifumin/dotfiles)
* Zsh 5.0.8
* Oh-My-Zsh
* peco
* tmux 2.0
* vim 7.4
* Nginx
* MySQL 5.6
* rbenv

## Prerequired
* Ansible
* Vagrant
* Virual Box

## Usage (Build a development environment)

```
$ git clone git@github.com:shifumin/vagrant-ansible-centos.git
$ cd vagrant-ansible-centos
$ vagrant up
```
