
# Login

```
az login
```

# Create a new resource group

```
data "azurerm_resource_group" "this" {
  name = "RG_AzureLab_20211217"
}

output "id" {
  value = data.azurerm_resource_group.this.id
}
```

# Terraform run

```
terraform fmt
terraform validate

terraform init
terraform plan
terraform apply

terraform output -raw tls_private_key
```