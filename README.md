# Create an Azure Key Vault

![Azure Public Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/PublicLastTestDate.svg)
![Azure Public Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/PublicDeployment.svg)

![Azure US Gov Last Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/FairfaxLastTestDate.svg)
![Azure US Gov Last Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/FairfaxDeployment.svg)

![Best Practice Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/BestPracticeResult.svg)
![Cred Scan Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/CredScanResult.svg)

![Bicep Version](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/BicepVersion.svg)

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https://github.com/thecloudplatform/azure-key-vault/blob/d7347f94e3dc9197005670f7becdf60363490b0e/azuredeploy.json)

This template creates an Azure Key Vault and a secret stored inside the key vault. To learn more about how to deploy the template, see the [quickstart](https://docs.microsoft.com/azure/key-vault/secrets/quick-create-template) article.

Your Azure AD user object ID is needed by the template to configure permissions. The following procedure gets the object ID (GUID).

Run the following Azure PowerShell or Azure CLI command by select Try it, and then paste the script into the shell pane. To paste the script, right-click the shell, and then select Paste.

CLI
PowerShell
Azure CLI

Copy

Try It
echo "Enter your email address that is used to sign in to Azure:" &&
read upn &&
az ad user show --id $upn --query "objectId" &&
echo "Press [ENTER] to continue ..."
Write down the object ID. You need it in the next section of this quickstart.
