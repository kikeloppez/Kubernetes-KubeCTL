# Instalar Portainer en Minikube

Primero debemos instalar los paquetes necesarios.

```sudo apt-get install ca-certificates curl gnupg lsb-release wget apt-transport-https  -y```

Con permisos Root descargamos helm y kubectl con snap para crear espacio de Portainer

```snap install helm --classic```

```snap install kubectl --classic```

![1](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/1.png)
![2](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/2.png)

Añadimos los repositorios de portainer.

```helm repo add portainer https://portainer.github.io/k8s/```

Actualizamos repositorios.

```helm repo update```

![3](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/3.png)

Sin permisos root creamos el servicio de Portainer con el siguiente comando.

```kubectl apply -n portainer -f https://downloads.portainer.io/ee2-18/portainer.yaml```

![4](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/4.png)

Visualizamos la IP de Minikube y la usamos para entrar al Dashboard de Portainer.

```minikube ip```

![5](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/5.png)

Portainer usa el puerto 3077.

![6](https://github.com/kikeloppez/Kubernetes-KubeCTL/blob/main/contenido/dos/6.png)

:arrow_left: [VOLVER](https://github.com/kikeloppez/Kubernetes-KubeCTL)
