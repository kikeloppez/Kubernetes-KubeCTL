# Instalar Portainer en Minikube

Primero debemos instalar los paquetes necesarios.

```sudo apt-get install ca-certificates curl gnupg lsb-release wget apt-transport-https  -y```

Con permisos Root descargamos helm y kubectl con snap para crear espacio de Portainer

```snap install helm --classic```

```snap install kubectl --classic```

![1]()
![2]()

Añadimos los repositorios de portainer.

```helm repo add portainer https://portainer.github.io/k8s/```

Actualizamos repositorios.

```helm repo update```

![3]()

Sin permisos root creamos el servicio de Portainer con el siguiente comando.

```kubectl apply -n portainer -f https://downloads.portainer.io/ee2-18/portainer.yaml```

![4]()

Visualizamos la IP de Minikube y la usamos para entrar al Dashboard de Portainer.

```minikube ip```

![5]()

Portainer usa el puerto 3077.

![6]()

:arrow_left: [VOLVER](https://github.com/kikeloppez/Kubernetes-KubeCTL)
