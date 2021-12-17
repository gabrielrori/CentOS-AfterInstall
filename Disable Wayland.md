



# Deshabilitar Wayland y configuring GNOME to use Xorg

Derechos de administrador

```sh
sudo su
```
Modificar el archivo de configuración, posible en 2 ubicaciones:
```sh
vi /etc/gdm3/custom.conf
vi /etc/gdm/custom.conf
```
En insert mode:
```sh
#WaylandEnable=false
```
Cambiar a:
```sh
WaylandEnable=false
```
Agregar la siguiente línea en la sección [daemon]:
```sh
DefaultSession=gnome-xorg.desktop
```


