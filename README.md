# Kubernetes Architecture

Kubernetes Evolution:
Kubernentes has evolved based on the drawbacks of Docker.
1) Clustering: Docker is single host platform and to handle multiple hosts or node Kuberenetes came up with "Cluster".
2) Auto Healing: There is no autohealing in dockers. If there is any issue with the running container, then the user has to manully fix or re-create new container.
3) Auto Scaling: Whenever the resource load is more then we need to do manual scaling in dockers.
4) Enterprise Level Support: Docker is very simple applicaton and to run any enterprise level of applications, we need,
   - Load Balancers
   - Firewalls
   - Autoscaling
   - Autohealing
   - API Gateways etc.

### Kubernetes Architecture
> Kubernetes has two types of Nodes and, Kubernetes will have multiple Master Nodes and multiple Worker Nodes. 
  1) Master Node => Also called as Control Plane (Controls the actions)
  2) Worker Node => Also called as Data Plane (Executes the actions)
     

> Control Plane	Data Plane
	
<img width="351" height="59" alt="image" src="https://github.com/user-attachments/assets/98db22ed-0504-4608-afd6-f8374ad6bb9b" />
