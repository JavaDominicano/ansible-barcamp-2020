# ansible-barcamp-2020
Ansible Demo BarCamp 2020

> Nota: Todas estás pruebas fueron ejecutadas en Debian versión 10 usando ansible 2.10.3

### Instalación de Ansible
> Nota: Ansible debe ser instalado solo en el servidor controlador.

```shell
# Instalar el manejador de paquetes de python
apt install python3-pip

# mediante pip instalamos ansible (Forma recomendada)
pip3 install ansible
```
[Documentación oficial instalación Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)


### Ad hoc command
```shell
# verify if the hosts are reachable
ansible webservers -i hosts.yml -m ping

# get hosts facts
ansible webservers -i hosts.yml -m setup | less
ansible webservers -i hosts.yml -m setup -a "filter=ansible_distribution*"
```

### Demo

- [Demo 01](webcluster-01/README.md)
- [Demo 02](webcluster-02/README.md)
- [Demo 03](webcluster-03/README.md)
![Demo 03](webcluster-03/demo_03.png)

### Recursos
- https://docs.ansible.com/ansible/latest/index.html
