Il faut installer les modules ansible-galaxy :  cisco.ios


quick install procedure : 

```
apt install ansible
ansible-galaxy collection install cisco.ios
apt install python3-paramiko


let's roll ! ;)

```


ensuite ansible-playbook -i inventory.ini playbook.yaml

et tout sera écrit dans le dossier backups/
