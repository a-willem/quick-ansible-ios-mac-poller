Il faut installer les modules ansible-galaxy :  cisco.ios

=== Known issues ===

Ansible v1.19 has some incompatibilties with netcommons.

The actual proposed workaround is to include : 

```
[all:vars]
ansible_network_import_modules=false
```
in your `inventory` file.


=== quick install procedure ===

```
apt install ansible
ansible-galaxy collection install cisco.ios
apt install python3-paramiko


let's roll ! ;)

```

ensuite ansible-playbook -i inventory.ini playbook.yaml

et tout sera écrit dans le dossier backups/
