Learn Kubernetes

What is Kubernetes?
Kubernetes provides a platform for deploying, scaling and managing containerized applications.
It offer features such as servicediscovery, rollingupdates and automated scaling.
Key features:
Pods: Pods are the smallest deployable unit in kubernetes encapsulating one or more containers.It makes effortless to manage multi-container applications.
Deployment, ReplicationController, Replicasets ensures that a specific number of replicas for the pods are running at all times.

Ex: a pod with two containers looks like

apiVersion: v1
kind: Pod
metadata:
  name: pod-with-two-containers
spec:
  containers:
  - name: container1
    image: image1
  - name: container2
    image: image2


Kubernetes assign each pod its unique IP address ensuring communication across pods
Service, Ingress and network policies provide different level of network abstraction

It offers a standardized way of managing storage systems. storageclasses, persistent volumes provides dynamic provisioning access controls.

Kubernetes can  automate the scaling of pods based on cpu or memory usage ensuring optimal resource allocation and performance.
Horizontal pod autoscaler HPA dynamically scales the number of replica pods in deployments, replicaset.
