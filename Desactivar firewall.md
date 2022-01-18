# Desactivar firewalls en CentOS 8
Luego de la instalación de CentOS, desactivar el firewall para permitir la comunicación por ssh, programa de monitoreo y configuración de clusters
Permisos de administrador:
```sh
sudo su
```
Estado del firewall:
```sh
systemctl status firewalld
```
Detener y deshabilitar firewall:
```sh
sudo systemctl stop firewalld
```
```sh
sudo systemctl disable firewalld
```
Comprobar que se detuvo el firewall (dead):
```sh
sudo systemctl status firewalld
```
----------------------------------------------------------------------------
