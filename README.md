# KubernetesPodProject
***
Simple kubernetes pod manifect creating 2 containers - nginx and tomcat. 

## 💻 Pre-requisites

Before you use this project you need to have Docker installed in your computer,and also Minikube.

https://www.docker.com/products/docker-desktop/
https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download

### Git clone
This will clone the project:
```
$ git clone https://github.com/Kar1stan/KubernetesPodProject.git
$ cd KubernetesPodProject
```

## 🚀 Run the manifest: 
To run the pod,open the terminal and run:
```
$ kubectl apply -f pod-myweb-v1.yaml
```
To delete pod,open the terminal and run:
```
$ kubectl delete -f pod-myweb-v1.yaml
```
To show detail of the pod,open the terminal and run:
```
$ kubectl describe pods my-web
```
To connect IP and open server locally,open the terminal and run:

To nginx container:
```
$ kubectl port-forward my-web 8888:80
```
To tomcat container:
```
$ kubectl port-forward my-web 8888:8080
```
