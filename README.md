# Azure naming module

This Terraform module is designed to help you to generate name for your Azure ressources.

It's a simplied version of this module : [Azure/terraform-azurerm-naming](https://github.com/Azure/terraform-azurerm-naming)

## Usage

```
module "azure_naming" {
  source  = "azurerm/naming/azure"
  version = "x.x.x"  
}
```