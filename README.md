# Azure-Storage-Assignment-01
## Creating an Azure storage via CLI command

Definition of Azure Storage Account

An Azure storage account contains all of your Azure Storage data objects: blobs, files, queues, and tables. 
The storage account provides a unique namespace for your Azure Storage data that's accessible from anywhere in the world over HTTP or HTTPS.

# Steps to Create a Storage Account on Azure Portal via CLI command

1. Create a resource group for your storage account using the az group create command. 
For example: az group create --name myResourceGroup --location eastus

2. Create a storage account using the az storage account create command. You need to specify a unique name for your storage account, the resource group name, the location, the storage account type, and the redundancy option. For example: az storage account create --name mystorageaccount --resource-group myResourceGroup --location eastus --sku Standard_LRS --kind StorageV2

3. You can verify that your storage account is created by using the az storage account show command. For example: az storage account show --name mystorageaccount --resource-group myResourceGroup.

4. Congratulatios! you have successfully created a resource group and a storage account via the CLI command.

  # Steps to delete the Resource  and Storage Account  via the CLI command

1.  To delete the storage account created via CLI, you can use the az storage account delete command.
  You need to specify the name of the storage account and the resource group that it belongs to. 
  For example, if you created a storage account named mystorageaccount in a resource group named myResourceGroup, 
  you can use the following command to delete it:

2. az storage account delete --name mystorageaccount --resource-group myResourceGroup

3. You will be prompted to confirm the deletion before it proceeds.
 You can also use the --yes or -y option to skip the confirmation.
 For more information and examples, you can check out the following source:

.az storage account | Microsoft Learn


