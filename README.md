# Kubernetes: Minikube and k9s
In this project, we will install and run Kubernetes using Minikube. 

* Minikube
https://minikube.sigs.k8s.io/docs/
* K9S:
https://k9scli.io/

## Step1:
Install Minikube to run the kubernetes cluster and Pods on it:
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```
## Step 2: Start Minikube
### minikube start

* **Note**:
Minikube can use Docker as a driver to run on it. So, if you get any error regarding the drive, do as follow:
Install Docker:
```
sudo apt install docker.io
```
Set the Driver and start Minikube:
```
minikube start --driver=docker
```
* **Out put:**
```
azizi@azizi-lab:~$ minikube start --driver=docker
😄  minikube v1.35.0 on Ubuntu 22.04 (vbox/amd64)
✨  Using the docker driver based on existing profile
👍  Starting "minikube" primary control-plane node in "minikube" cluster
🚜  Pulling base image v0.0.46 ...
🔄  Restarting existing docker container for "minikube" ...
🐳  Preparing Kubernetes v1.32.0 on Docker 27.4.1 ...
🔎  Verifying Kubernetes components...
    ▪ Using image gcr.io/k8s-minikube/storage-provisioner:v5
🌟  Enabled addons: storage-provisioner, default-storageclass
🏄  Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default
```



  
