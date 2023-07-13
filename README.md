# az-aks
Creating an AKS cluster on Azure using Terraform

### To login in Azure use az cli
``` bash
az login --use-device-code
```

### Update Kubeconfig
``` bash
az aks get-credentials --resource-group [name] --name [aks-name]
```

### Login in ACR
``` bash
az acr login --name [acr-name]
```

### Create permissions to AKS access ACR
``` bash
az aks update -n [aks-name] -g [rs-name] --attach-acr [acr-name]
```

What's inside [ ] replace for your environment.
