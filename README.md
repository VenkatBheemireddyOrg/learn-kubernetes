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
     

Control Plane	Data Plane
"1) API Server
2) etcd
3) Scheduler
4) Controller Manager
5) Cloud Controller Manager"	"1) Kubelet
2) Kubelet-proxy
3) Container Runtime"
<img width="690" height="175" alt="image" src="https://github.com/user-attachments/assets/274009cb-17f2-4092-ab4a-16538bb96582" />

