---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "planetscale_database Data Source - terraform-provider-planetscale"
subcategory: ""
description: |-
The database data source allows you to retrieve a single database from an organization
---

# planetscale_database (Data Source)
The database data source allows you to retrieve a single database from an organization

## Example Usage

```terraform
data "planetscale_database" "db" {
  organization = "yourplanescaleorg"
  name = "your planetscaledb"
}
output "database" {
  value = data.planetscale_database.db.region
}
```
## Argument Reference
- `organization`  - Organization the database is under
- `name` - Name of the database

## Attributes Reference

In addition to all the arguments above, the following attributes are exported.

- `name` (string) name of the database
- `created_at` (String)
- `notes` (String) notes assosicated with this database
- `region` (Map of String) region information
- `updated_at` (String)
- `last_updated` (String)




