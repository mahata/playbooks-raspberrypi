# playbooks-raspberrypi

Ansible Playbooks to provision my personal Raspberry Pis.

You won't be able to run the entire playbooks because my Ansible Vault Key is needed for some commands.

(In Progress)

## Prerequisites

* Ansible: Version 1.9.x

## Provision

### Common Playbooks

```sh
ansible-playbook -vv -i inventories/raspberrypi common.yml
```

### Playbook for pi1

```
ansible-playbook -vv -i inventories/raspberrypi --limit=frontend pi1.yml
```

### Playbook for pi2

```
ansible-playbook -vv -i inventories/raspberrypi --limit=frontend pi2.yml
```

## Note

On my environment, there're lines as follows in `/etc/hosts`:

```
192.168.1.23    pi1
192.168.1.30    pi2
```
