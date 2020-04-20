# PostmanCollectionForAzureDevopsRestAPIs
Postman Collection For Azure Devops RestAPIs

First A service connection needs to be created
Reference Doc: https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli?toc=%2Fazure%2Fazure-resource-manager%2Ftoc.json&view=azure-cli-latest
AZ CLI:
Az login
az ad sp create-for-rbac --name SPCommithistory
Changing "SPCommithistory" to a valid URI of "http://SPCommithistory", which is the required format used for service principal names
Creating a role assignment under the scope of "/subscriptions/4af51c74-d4f6-4a7c-9ac1-14ea6a6b4274"
  Retrying role assignment creation: 1/36


az account list --output table --query '[].{Name:name, SubscriptionId:id, TenantId:tenantId}'

az account show --query id

