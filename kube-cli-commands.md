### install  minikube and kubectl
`sudo apt update`

`curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64\nsudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64`

`curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"`

`sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl`

`minikube start`

`kubectl`

`minikube`

### create minikube cluster
`minikube start`

`kubectl get nodes`

`minikube status`

`kubectl version`

### delete cluster and restart in debug mode
`minikube delete`

`minikube start --alsologtostderr`

`minikube status`

### kubectl commands
`kubectl get nodes`

`kubectl get pod`

`kubectl get services`

`kubectl create deployment {deployment-name} --image=nginx`

`kubectl get deployment`

`kubectl get replicaset`

`kubectl edit deployment {deployment-name}`

### debugging
`kubectl logs {pod-name}`

`kubectl exec -it {pod-name} -- bin/bash`

### create mongo deployment
`kubectl create deployment {deployment-name} --image=mongo`

`kubectl logs {pod-name}`

`kubectl describe pod {pod-name}`

### delete deployment
`kubectl delete deployment {deployment-name}`


### create or edit config file
`vim nginx-deployment.yaml`

`kubectl apply -f nginx-deployment.yaml`

`kubectl get pod`

`kubectl get deployment`

### delete with config
`kubectl delete -f nginx-deployment.yaml`

#Metrics

`kubectl top` The kubectl top command returns current CPU and memory usage for a cluster’s pods or nodes, or for a particular pod or node if specified.




