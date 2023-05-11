# Kubernetes

## Minikube setup


## Install docker

```sh
sudo apt-get update
sudo apt-get install docker.io -y
sudo apt-get update
sudo usermod -aG docker $USER && newgrp docker 
```

## Install Minikube
```sh
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

## Install kubectl
```sh
sudo curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
sudo chmod +x kubectl
sudo mv kubectl /usr/local/bin/
```

## Start Minikube
```sh
minikube start --driver=none
```
