#Programas básicos
Actualizar los paquetes y volver a cargar el repositorio
```sh
sudo dnf update -y 
```
Instalar el repositorio EPEL (Extra Packages for Enterprise Linux)
```sh
sudo dnf install epel-release
```
## Wget

Instalar wget
```sh
sudo dnf install wget
```
## Zoom

Descargar el .rpm de zoom para Centos 64 bits
```sh
wget https://zoom.us/client/latest/zoom_x86_64.rpm
```
Instalar archivo .rpm en el sistema
```sh
sudo dnf localinstall zoom_x86_64.rpm
```
Revisar versión instalada
```sh
rpm -qi zoom
```
