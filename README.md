# ARM-IaC-Storage-Sample
This is sample to deploy azure storage account via Azure ARM template.

# Prerequiste

1.Install Azure CLI via below link.
https://learn.microsoft.com/zh-tw/cli/azure/install-azure-cli-windows?tabs=azure-cli
<br>
2.Login into Azure via Azure cli.
"az login"
# How to use it?

1.Create resource group.
<br>
"az group create --name {your resource group name} --location {your resource group location}"
![image](https://github.com/Wayne5888/ARM-IaC-Storage-Sample/assets/63963809/3e03900b-0145-4ef9-97b2-0c9f969305b4)
<br>
2.Validate arm template file.
<br>
"az group deployment validate -g {your resource group name} --template-file .\deployStorage.json --parameters .\deployStorage.params.json"
![image](https://github.com/Wayne5888/ARM-IaC-Storage-Sample/assets/63963809/d53d5c2c-1b36-47b8-8878-a8ca2564aa6f)
<br>
3.If above is success, then create resource.
<br>
"az group deployment create -g demo3 --template-file .\deployStorage.json --parameters .\deployStorage.params.json"
![image](https://github.com/Wayne5888/ARM-IaC-Storage-Sample/assets/63963809/c9438276-84d4-49ad-878a-9b268d576964)
<br>
You may see deploy success in resource group page in azure.
![image](https://github.com/Wayne5888/ARM-IaC-Storage-Sample/assets/63963809/56319a02-2302-437c-8c82-9c477e31cfea)





