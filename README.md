# Ansible

## Ping

- `ssh-add -K {{private_key}}`
- `ansible ansible -i compute_engine.inv -m ping all -u {{login_user}}`
- `ansible ansible -i compute_engine.inv -m ping all -u {{login_user}} --private-key {{path_to_private_key}}`

## git install command

- `ansible -i compute_engine.inv -m apt -a "name=git state=latest update_cache=yes" all -u {{login_user}} --become`

## docker install playbook

- `ansible-playbook -i inventory com.yaml`