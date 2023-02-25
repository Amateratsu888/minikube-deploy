# Minikube-deploy
### Deployment of deno api rest with minikube 

 - install **vagrant**
 - put on the file **Vagrantfile** and launch **vagrant up** and after **vagrant ssh** command this will create a virtual machine where we will already install minikube, clusterand logging you via ssh
 - add the ingress addons with the command **minikube addons enable ingress**
 - then copy the ingress, deployment, and service  yaml files and at the level of our virtual machine then make a **kubectl apply -f file.yaml** of each file
 - to get access outside the VM do a **kubectl port-forward  service/ingress-name External Port:Target Port**
