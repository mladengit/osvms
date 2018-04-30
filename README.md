Dependencies:

* VirtualBox + VirtualBox Extension Pack
* vagrant
* python3

apt install libssl-dev
pip3 install -r requirements.txt
ansible-galaxy install -r roles.yml

Start:

```
vagrant up [<machine_name>]
```

Provision:

```
ansible-playbook <playbook>
```
