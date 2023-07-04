# Create a new Storage Account

- Set variables for the resource group and storage account names

```azurecli
resourceGroupName="<RESOURCE_GROUP_NAME>"
storageAccountName="<STORAGE_ACCOUNT_NAME>"
```

- Create a new resource group

```azurecli
az group create --name $resourceGroupName --location eastus
```

- Create a new storage account in the resource group

```azurecli
az storage account create --name $storageAccountName --resource-group $resourceGroupName --location eastus --sku Standard_LRS --kind StorageV2
```

## Try it out

[![Launch Cloud Shell](https://learn.microsoft.com/azure/cloud-shell/media/embed-cloud-shell/launch-cloud-shell-1.png)](https://shell.azure.com)
