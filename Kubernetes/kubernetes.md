# Kubernete and Azure Kubernetes Service (AKS) Commands

## Local Kubernetes (kubectl)

| Command                              | Description                                       |
|--------------------------------------|---------------------------------------------------|
| `kubectl get svc`                    | Get a list of services in the Kubernetes cluster. |
| `kubectl delete svc`                 | Delete a service in the Kubernetes cluster.       |
| `kubectl delete deployment appName`  | Delete a deployment with the specified name.     |
| `kubectl create deployment appName --image=imageName:v1 --replicas=2` | Create a deployment with 2 replicas. |
| `kubectl expose deployment appName --type=LoadBalancer --port=8080 --target-port=80` | Expose a deployment as a LoadBalancer service. |
| `kubectl get pods`                   | List pods in the Kubernetes cluster.              |

### Troubleshooting in Local Kubernetes

| Command                               | Description                                       |
|---------------------------------------|---------------------------------------------------|
| `kubectl logs podName`                | View container logs for a specific pod.          |
| `kubectl exec -it podName -- /bin/sh` | Start an interactive shell in a running pod.     |
| `kubectl get events`                  | List cluster events for debugging.               |

## Azure Kubernetes Service (AKS)

| Command                                        | Description                                       |
|------------------------------------------------|---------------------------------------------------|
| `az account show`                              | Display information about the Azure subscription. |
| `az configure --defaults group=resourseGroup`  | Set the default resource group for Azure CLI.    |
| `az aks get-credentials --name k8sServiceName` | Set up credentials for accessing AKS cluster.    |
| `kubectl config current-context`                | Check the current AKS cluster context.           |
| `kubectl get nodes`                            | Get a list of nodes in the AKS cluster.          |
| `kubectl get deployments`                      | List deployments in the AKS cluster.            |
| `kubectl get pods`                             | List pods in the AKS cluster.                   |
| `kubectl get service`                          | List all services in the AKS cluster.            |

### Troubleshooting in Azure Kubernetes Service (AKS)

| Command                               | Description                                       |
|---------------------------------------|---------------------------------------------------|
| `kubectl logs podName`                | View container logs for a specific pod.          |
| `kubectl exec -it podName -- /bin/sh` | Start an interactive shell in a running pod.     |
| `kubectl get events`                  | List cluster events for debugging.               |
| `kubectl get svc -n kube-system`      | List services in the `kube-system` namespace.    |
| `kubectl describe node nodeName`      | Get details about a specific node in the AKS cluster. |
| `kubectl describe pod podName`        | Get detailed information about a specific pod.   |
| `kubectl describe service serviceName` | Get details about a specific service.             |

Please note that these commands are for common Kubernetes and AKS operations and can be customized for specific use cases.
