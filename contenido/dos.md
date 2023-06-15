# Instalación de Minikube

Todos los comandos han sido sacados de la página oficial de [Minikube](https://minikube.sigs.k8s.io/docs/start/).

Nos descargamos los paquetes necesarios.

```apt install curl```

Instalamos virtual box.

```apt install virtualbox```

En caso de no poder instalarlo mediante el comando anterior, seguir este [enlace](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/uno/cuatro.md).

Descargamos el paquete de minikube.

```curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64```

Y lo instalamos.

```sudo install minikube-linux-amd64 /usr/local/bin/minikube```
![1](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/uno/1.png)

Iniciamos Minikube con el siguiente comando. Importante hacerlo sin privilegios root.

```minikube start```

![2](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/uno/2.png)

:arrow_left: [VOLVER](https://github.com/kikeloppez/Kubernetes-KubeCTL)
