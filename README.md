# kubernetes

Setup a self managed kubernetes cluster with containerd for training.

To check cluster components:  
`kubectl get --raw='/readyz?verbose'`

After installation of kubernetes in order to be able to monitor resources of run this command:  
`kubectl appy -f metrics.yaml`

Use below commands to check pod and node resource usage:

`kubectl top nodes`  
`kubectl top nodes -n kube-system`  
`kubectl top pods -n kube-system`

To install latets helm chart run these commands as root:

`curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3`  
`chmod 700 get_helm.sh`  
`./get_helm.sh`
