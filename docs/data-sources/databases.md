---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "planetscale_databases Data Source - terraform-provider-planetscale"
subcategory: ""
description: |-
The database data source resource allows you to retrieve all databases from an organization
---

# planetscale_databases (Data Source)
The database data source allows you to retrieve all databases from an organization

## Example Usage

```terraform
data "planetscale_databases" "all" {
  organization = "yourplanescaleorg"
}
output "database" {
  value = data.planetscale_database.all.databases
}
```

## Argument Reference
- `organization`  - Organization the databases are under

## Attributes Reference

In addition to all the arguments above, the following attributes are exported.

- **databases** (List of Object) (see [below for nested schema](#nestedatt--databases))

<a id="nestedatt--databases"></a>
### Nested Schema for `databases`

Read-Only:

- **created_at** (String)
- **name** (String)
- **notes** (String)
- **region** (Map of String)
- **updated_at** (String)

