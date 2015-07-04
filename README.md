# Provision a web app with a SQL Database

For information about using this template, see [Provision a web app with a SQL Database](https://azure.microsoft.com/en-us/documentation/articles/app-service-web-arm-with-sql-database-provision/).
<br>
New-AzureResourceGroup -DeploymentName 'AzureDeploy' -Location 'West US' -TemplateUri 'https://raw.githubusercontent.com/cliveg/azure-quickstart-templates/master/active-directory-new-domain/azuredeploy.json' -Verbose -Name clivegadvm -newStorageAccountName clivegadvm -VirtualNetworkName clivegAdVNET -AdminUserName AzAdmin -AdminPassword (ConvertTo-SecureString 'AzP@ssword1' -AsPlainText -Force) -domainName contoso.com -addnsname aad -locationFromTemplate 'West US'
