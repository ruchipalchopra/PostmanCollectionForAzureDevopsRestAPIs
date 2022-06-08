# PostmanCollectionForAzureDevopsRestAPIs
Postman Collection For Azure Devops RestAPIs

First A service connection needs to be created
Reference Doc: https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli?toc=%2Fazure%2Fazure-resource-manager%2Ftoc.json&view=azure-cli-latest

AZ CLI Commands to use:
Az login
az ad sp create-for-rbac --name SPCommithistory

az account list --output table --query '[].{Name:name, SubscriptionId:id, TenantId:tenantId}'

az account show --query id

