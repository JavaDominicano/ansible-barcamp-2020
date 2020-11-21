# ansible-barcamp-2020
Ansible Demo BarCamp 2020

> Nota: Todas estás pruebas fueron ejecutadas en Debian version 10 y ansible 2.10.3

### Instalacion de Ansible
> Nota: Ansible solo hay que instalarlo en servidor controlador.

```shell
# Instalar el instalador de paquetes de python pip
apt install python3-pip

# mediante pip instalar ansible (Manera que recomiendo)
pip3 install ansible
```
[Documentación oficial instalación Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)


### Ad hoc command
```shell
# verify if the hosts are reachable
ansible proxy -i host -m ping

# get hosts facts
ansible proxy -i host -m setup | less
ansible proxy -i host -m setup -a "filter=ansible_distribution*"
```

### Demo

- [Demo 01](webcluster-01/README.md)
- [Demo 02](webcluster-02/README.md)
- [Demo 03](webcluster-03/README.md)

### Recursos
- https://docs.ansible.com/ansible/latest/index.html
