# Azure Function App and API Management Terraform Module

This module is used to create an Azure function app and API management service using Terraform.

## Description

The module sets up the following resources:
- Azure resource group
- Azure storage account
- Azure app service plan
- Azure function app
- Azure API management
- Azure API management API

## Prerequisites

- Terraform >= v0.12.6
- Azure CLI

## Provider
This module requires the AzureRM provider. Make sure you have version 3.0.0 installed.

## Inputs

No input variables are required for this module to run. All variable values are pre-defined in the code. 

## Usage

Clone the repository to your local machine and change into the directory containing the Terraform files:

```bash
git clone https://github.com/Susmita86/azure-demo/
cd azure-demo
```

```bash
terraform init
```

```bash
terraform plan
```

```bash
terraform apply
```
You will be prompted to confirm that you want to create the infrastructure.

Outputs
The module has no explicit outputs, but once the infrastructure is set up, you can query for information about the resources using the Azure CLI or through the Azure portal.

Note
The terraform will create the following resources:

Resource Group named function-rg in the West Europe region.
Storage Account named myfastorageaccount within the above resource group.
App Service Plan named my-function-app-plan within the above resource group.
Function App named susmita-function-app within the above resource group.
API Management named susmitasen-apim within the above resource group.
API Management API named example-api within the above API Management.
Please remember to replace the hardcoded values with your actual requirement. Especially replace company@terraform.io with your actual email.

License
This project is licensed under the terms of the MIT license.

Issues
If you encounter an issue or have a question, feel free to open an issue. We welcome contributions, so feel free to fork the repository and contribute.