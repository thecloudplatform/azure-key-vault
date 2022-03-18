# Create an Azure Key Vault

![Azure Public Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/PublicLastTestDate.svg)
![Azure Public Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/PublicDeployment.svg)

![Azure US Gov Last Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/FairfaxLastTestDate.svg)
![Azure US Gov Last Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/FairfaxDeployment.svg)

![Best Practice Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/BestPracticeResult.svg)
![Cred Scan Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/CredScanResult.svg)

![Bicep Version](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.keyvault/key-vault-create/BicepVersion.svg)

[![Deploy To Azure]
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fthecloudplatform%2Fazure-key-vault%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

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
