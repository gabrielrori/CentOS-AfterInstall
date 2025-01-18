

# Instalación de drivers de NVIDIA y CUDA en RPM Linux

## Actualizar Linux


Actualizar repositorios y paquetes de linux
```sh
sudo dnf upgrade --refresh -y
```

## Preinstalar dependenciaas 

Importar EPEL (Extra Packages for Enterprise Linux) 
```sh
sudo dnf install epel-release -y
```
Agregar repositorio de Nvidia
```sh
sudo dnf config-manager --add-repo https://developer.download.nvidia.com/compute/cuda/repos/rhel8/x86_64/cuda-rhel8.repo
```
Instalar los kernel-devel y headers que usará los drivers de Nvidia
```sh
sudo dnf install kernel-devel-$(uname -r) kernel-headers-$(uname -r)
```
## Instalación de drivers de Nvidia
```sh
sudo dnf install nvidia-driver nvidia-settings
```

## Instalación de los drivers de CUDA
```sh
sudo dnf install cuda-driver
```
Presionar "y"
```sh
reboot now
```

## Luego de instalar verificar instalación
```sh
nvidia-smi
```
## Instalación de Neofetch

```sh
sudo dnf install neofetch -y
```
```sh
neofetch
```

----------------------------------------------------------------------------

