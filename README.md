# Ansible Role: Dotfiles

[![Build Status](https://travis-ci.org/issmirnov/ansible-role-dotfiles.svg?branch=master)](https://travis-ci.org/issmirnov/ansible-role-dotfiles)

Automated dotfile installer script.

## Requirements

A valid dotfiles repo with a single install command.

## Role Variables

```
dotfiles_repo_url:
dotfiles_target_dir:
dotfiles_install_command:
dotfiles_update: yes # pull in latest changes
dotfiles_update_command: git pull
```

## Example Playbook

```
- hosts: servers
  vars:
    dotfiles_repo_url: https://github.com/username/dotfiles.git
  roles:
    - { role: issmirnov.dotfiles}
```

## License

MIT

## Author Information

Ivan Smirnov, http://ivansmirnov.name
