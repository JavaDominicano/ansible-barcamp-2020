# ansible-barcamp-2020
Ansible Demo BarCamp 2020

### Ad hoc command
```shell
# verify if the hosts are reachable
ansible proxy -i host -m ping

# get hosts facts
ansible proxy -i host -m setup | less
ansible proxy -i host -m setup -a "filter=ansible_distribution*"
```
