# Instalar VirtualBox - Opción 2

Accedemos a la página oficial de [VirtualBox](https://www.virtualbox.org/wiki/Linux_Downloads).
![1]()

Cogemos el enlace de la version que vayamos a usar, en mi caso Ubuntu 22.04.
Descargamos el paquete mediante el siguiente comando.

```wget https://download.virtualbox.org/virtualbox/7.0.8/virtualbox-7.0_7.0.8-156879~Ubuntu~jammy_amd64.deb```
![2]()

Ejecutamos el siguiente comando para arreglar dependencias.

```apt --fix-broken install```

Para instalarlo usamos el siguiente comando.

```dpkg -i virtualbox-7.0_7.0.8-156879~Ubuntu~jammy_amd64.deb```
![3]()

Con esto ya estaría instalado, lo comprobamos.
![4]()
