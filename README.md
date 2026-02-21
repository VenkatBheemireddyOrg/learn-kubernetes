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
     

> Data Plane Components: Kuberenetes Data Plane has 3 components.
   1) Kubelet: Kubelet is responsible for deploying and creating pods. It will ensure the pods are running without any issues. In case of any issues, it will inform to API Server.
   2) Kubelet proxy: Kubelet proxy is responsible for creating Network, assigning IP Addresses and Load Balancing.
   3) Container Runtime: Cotainer Runtime is responsible for running containers.

> Control Plane Components: Kubernetes Control Plane has 5 components.
   1) API Server: API server receives the request and sends the request to Data Plane.
   2) Kube Scheduler: This is responsible for scheduling resources on k8s.
   3) etcd: etcd is basically a key-value store, and the entire kuberenetes cluster information is stored as objects or key-value pairs inside etcd.
   4) Controller Manager: Kubermetes supports autoacaling. To support auto-scaling Kubernetes has components like Controllers. ReplicaSet is one of the Kubernetes Controllers.
   5) Cloud Controller Manager (CCM):
      - If we are running Kubernetes on on-premise then CCM is not required. CCM is required if we are running Kubernetes on cloud (EKS/AKS/etc)
      - Whenever user wants to create resources (like load balancer, storage, etc) on cloud then Kubernetes use CCM to translate the request into respective API cloud request. So for this conversion, Kubernetes uses CCM.
        


