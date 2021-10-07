---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "planetscale_organizations Data Source - terraform-provider-planetscale"
subcategory: ""
description: |-
The organization data source allows you to retrive all organizations asssociated with your account 
---

# planetscale_organizations (Data Source)

The organization data source allows you to retrive all organizations asssociated with your account 


## Example Usage

```terraform
data "planetscale_organizations" "orgs" {}

output "organizations" {
  value = data.planetscale_organizations.orgs.organizations
}
```

### Read-Only

- **organizations** (List of Object) (see [below for nested schema](#nestedatt--organizations))

<a id="nestedatt--organizations"></a>
### Nested Schema for `organizations`

Read-Only:

- **created_at** (String)
- **name** (String)
- **updated_at** (String)

