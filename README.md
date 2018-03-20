Dependencies:
* VirtualBox + VirtualBox Extension Pack
* vagrant
* python2

apt install libssl-dev
pip install -r requirements.txt

Start:
```
vagrant up [<machine_name>]
```

Provision:
```
ansible-galaxy install -r roles.yml
ansible-playbook <playbook>
```
