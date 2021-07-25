# EP7 - Deploy multiple Azure environments with the same code base - Terraform (TFVars)

In this episode, I will show you how deploy multiple environments with the same code base!

## Scripts

See [ep4_azure_lab_terraform/scripts](https://github.com/someoneelsescloud/ep4_azure_lab_terraform/tree/master/scripts) for the following scripts to get started:

|Name|Description|
|---|---|
|.\scripts\Clean-Terraform|Clean up Terraform working folders - Terraform init will restore the folder|
|.\scripts\Create-TFServicePrincipal|Create Service Principal for Terraform|
|.\scripts\Install-Terraform|Downloading and configure Terraform open source|
|.\scripts\Uninstall-AzModule|Uninstall the Az Module - Script above requires AzureRM|


## Single-Deploy Terraform Configuration
We will be reusing the [Single Deployment](https://github.com/someoneelsescloud/ep4_azure_lab_terraform/tree/master/lab/single-deploy) code from [EP4: Build an Azure Lab with Terraform](https://github.com/someoneelsescloud/ep4_azure_lab_terraform)

This is a simplied Terraform deployment, where by all the configuration files are within the single folder i.e. a Terraform workspace. However the code has been refactored to use variable inputs which allow you to specify environment and region. The resource names have been updated to include the environment and tag have been added to specify environment specific details.
The following diagram shows all the components that will be deployed!
![single-deploy-diagram](_images/multi-env-deploy-v2.png)

Code Structure Summary:
![single-deploy-diagram](_files/file-structure-v2.png)

Document References:
- [Hashicorp - Terraform: Get Started - Azure](https://learn.hashicorp.com/collections/terraform/azure-get-started)
- [Input Variables](https://www.terraform.io/docs/language/values/variables.html)
- [Local Values](https://www.terraform.io/docs/language/values/locals.html)
- [Define Input Variables](https://learn.hashicorp.com/tutorials/terraform/azure-variables?in=terraform/azure-get-started)
- [Refactor Monolithic Terraform Configuration - Example is AWS but concept is the same!](https://learn.hashicorp.com/tutorials/terraform/organize-configuration)
- [What is the difference between variable.tf and variable.tfvars in Terraform?](https://amazicworld.com/difference-between-variable-tf-and-variable-tfvars-in-terraform/)
- 
## Full episode on here:
Website Link: https://www.someoneelsescloud.com/episodes/ep4-build-an-azure-lab-with-terraform

### Listen to the Audio Only version:

Google Podcasts: https://cutt.ly/ogvwqTl

Apple Podcasts: https://cutt.ly/YgvweNk

Spotify Podcasts: https://cutt.ly/igvwezs

Stitcher Radio: https://cutt.ly/ugvwewo

Tunein Radio: https://cutt.ly/Xgvwwpf

Visit the website for more information: www.someoneelsescloud.com

See all links to all platforms here: https://www.someoneelsescloud.com/links