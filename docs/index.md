---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "Provider: Planetscale"
subcategory: ""
description: |-
Terraform provider for interacting with Planetscale
---

# planetscale Provider
Unofficial [Planetscale](https://planetscale.com ) provider built out of curiosity. 

This provider currently allows users to:

- Create Planetscale databases
- Read Planetscale databases
- Read Planetscale organizations


## Example Usage

```terraform
provider planetscale{
    access_token = "yourplanetscaletoken"
}
```


<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **access_token** (String) access token used for authenticating against Planescale API