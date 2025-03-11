az login

az login --tenant 604c1504-c6a3-4080-81aa-b33091104187


az account list 
az account set --subscription ade79e45-e72d-49ad-8a7b-f86b98cd9d42

az configure --defaults group="learn-1dd9fbbe-31fd-4eb8-853f-e8688e33b537"


az deployment group create --name main --template-file main.bicep --parameters main.parameters.dev.json


testAdmin
testPassword123**(8)


az keyvault create --name my-key-vaault-test-kozh --location eastus2 --enabled-for-template-deployment true
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorLogin" --value testAdmin --output none
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorPassword" --value testPassword123**(8) --output none
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorPassword" --value 'testPassword123**(8)' --output none



az keyvault show --name my-key-vaault-test-kozh --query id --output tsv
/subscriptions/bbc84a72-5cd7-4d49-8727-eb647636cbc6/resourceGroups/learn-kozhevnikov3/providers/Microsoft.KeyVault/vaults/my-key-vaault-test-kozh

https://portal.azure.com/#browse/resourcegroups




==================


az account set --subscription bbc84a72-5cd7-4d49-8727-eb647636cbc6

az configure --defaults group=learn-kozhevnikov3
az configure --defaults group=learn-1dd9fbbe-31fd-4eb8-853f-e8688e33b537
az configure --defaults group='rg-learn-kozhevnikov4'
