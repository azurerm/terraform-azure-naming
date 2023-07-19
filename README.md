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

## Providers

random

## Modules

No modules.

## Resources

No resources.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| prefix | Not recommended - Prefix to add to the name of you resources. | `list(string)` | [] | no |
| suffix | Recommended - Suffix to add to the name of you resources. Please use only lowercase characters when possible. | `list(string)` | [] | no |
| unique-seed | Custom value for the random characters to be used. | `string` | "" | no |
| unique-length | Max length of the uniqueness suffix to be added. | `number` | 0 | no |
| unique-include-numbers | Include numbers in the unique generation. | `bool` | true | no |


## Outputs

| Name | Description |
|------|-------------|
