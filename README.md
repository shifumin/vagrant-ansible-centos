Vagrant-Ansible-CentOS
===============
This is Ansible playbook to provision a CentOS box suitable for production on a local Vagrant environment.

## Stack
* Git
* dotfiles (install my dotfiles based on https://github.com/shifumin/dotfiles)
* Zsh
* Oh-My-Zsh
* tmux
* vim
* rbenv

## Prerequired
* Ansible
* Vagrant
* Virual Box

## Usage(for CentOS6.6)

```
$ git clone git@github.com:shifumin/vagrant-ansible-rails.git
$ cd vagrant-ansible-rails
$ vagrant init chef/centos-6.6
$ vagrant up
```
