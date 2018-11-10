# ansible-shell

Ansible role to configure/add a shell.

[![Build Status](https://img.shields.io/travis/feffi/ansible-shell.svg)](https://travis-ci.org/feffi/ansible-shell) [![Github All Releases](https://img.shields.io/github/downloads/feffi/ansible-shell/total.svg)](https://github.com/feffi/ansible-shell) [![GitHub forks](https://img.shields.io/github/forks/feffi/ansible-shell.svg?style=social&label=Fork)](https://github.com/feffi/ansible-shell) [![GitHub stars](https://img.shields.io/github/stars/feffi/ansible-shell.svg?style=social&label=Star)](https://github.com/feffi/ansible-shell) [![GitHub watchers](https://img.shields.io/github/watchers/feffi/ansible-shell.svg?style=social&label=Watch)](https://github.com/feffi/ansible-shell) [![Twitter Follow](https://img.shields.io/twitter/follow/feffi1.svg?style=social&label=Follow)](https://twitter.com/feffi1) [![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/feffi/ansible-shell/blob/master/LICENSE)

## Role Defaults Variables

```yaml
ansible_shell:  [
  "zsh",
  "zsh-completions",
  "bash",
  "bash-completion"
]
```

Example:

```yaml
- hosts: all
  vars:
    ansible_shell:
      - "zsh"
      - "zsh-completions"
      - "bash"
      - "bash-completion"
  roles:
    - { role: ansible-shell }
```
