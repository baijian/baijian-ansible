Ansible Playbooks
===

The majority of these playbooks is to provide my development machines, including Max OSX Ubuntu Fedora and Gentoo.

### Playbook

Each playbook is composed of one or more 'plays' in a list. The goal of a play is to map a group of hosts to some well
defined roles, represented tasks. At a basic level, a task is nothing more than a call to an ansible module.But by
composing a playbook of multiple 'plays', it is possible to orchestrate multi-machine deployments, running certain
steps on certain steps. You can run different plays at different times.

### Quick Start

* for mac, *xcode* and *homebrew* should be installed first

* authorized_keys should be transferred to the remote hosts

$ ansible-playbook -i [hosts.xxx] playbook.yml

$ ansible-playbook --connection=local -i hosts.local --ask-sudo-pass development-playbook.yml --extra-vars "ansible_distribution=MaxOSX"

### TODO

* vim
* screen
* terminal
* ansible
* zsh
