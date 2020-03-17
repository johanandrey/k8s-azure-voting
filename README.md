Cloned from:

https://github.com/Azure-Samples/azure-voting-app-redis.git


- Build to Azure registry

az acr build --registry $ACR_NAME --image bgh-azure-vote-front:latest .

- Reference:

https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task

export ACR_NAME=bghk8sregistry
az aks update -n k8scluster -g k8sdev --attach-acr $ACR_NAME
