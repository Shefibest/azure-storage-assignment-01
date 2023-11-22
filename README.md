# Azure-Storage-Assignment-01
## Creating an Azure storage via CLI command

Definition of Azure Storage Account

An Azure storage account contains all of your Azure Storage data objects: blobs, files, queues, and tables. 
The storage account provides a unique namespace for your Azure Storage data that's accessible from anywhere in the world over HTTP or HTTPS.

STEPS TO CREATE A STORAGE ACCOUNT ON AZURE PORTAL VIA CLI

Create a resource group for your storage account using the az group create command. 
For example: az group create --name myResourceGroup --location eastus

Create a storage account using the az storage account create command. You need to specify a unique name for your storage account, the resource group name, the location, the storage account type, and the redundancy option. For example: az storage account create --name mystorageaccount --resource-group myResourceGroup --location eastus --sku Standard_LRS --kind StorageV2

You can verify that your storage account is created by using the az storage account show command. For example: az storage account show --name mystorageaccount --resource-group myResourceGroup
