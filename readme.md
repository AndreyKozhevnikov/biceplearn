az login

az login --tenant 604c1504-c6a3-4080-81aa-b33091104187


az account set --subscription 010fd40c-687a-4665-bfcf-04bffb0fbadd

az deployment group create --name main --template-file main.bicep --parameters main.parameters.dev.json


testAdmin
testPassword123**(8)


az keyvault create --name my-key-vaault-test-kozh --location eastus2 --enabled-for-template-deployment true
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorLogin" --value testAdmin --output none
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorPassword" --value testPassword123**(8) --output none
az keyvault secret set --vault-name my-key-vaault-test-kozh --name "sqlServerAdministratorPassword" --value 'testPassword123**(8)' --output none



az keyvault show --name my-key-vaault-test-kozh --query id --output tsv
/subscriptions/bbc84a72-5cd7-4d49-8727-eb647636cbc6/resourceGroups/learn-kozhevnikov3/providers/Microsoft.KeyVault/vaults/my-key-vaault-test-kozh


