Dependencies:
* VirtualBox
* vagrant
* ansible

Start:
```
vagrant up [<machine_name>]
```

Provision:
```
ansible-galaxy install -r roles.yml
ansible-playbook <playbook>
```
