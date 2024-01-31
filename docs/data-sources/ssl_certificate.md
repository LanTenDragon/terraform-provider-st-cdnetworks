---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "st-cdnetworks_ssl_certificate Data Source - st-cdnetworks"
subcategory: ""
description: |-
  This data source provides certificates configured in cdnetworks.
---

# st-cdnetworks_ssl_certificate (Data Source)

This data source provides certificates configured in cdnetworks.

## Example Usage

```terraform
data "st-cdnetworks_ssl_certificate" "certlist" {
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `cert_name_list` (List of String) List of certificate name.If cert_name_list is null,retrieve all certificates.If cert_name_list is not null (includes empty), retrive certificates with specific name.

### Read-Only

- `cert_list` (Attributes List) List of certificate (see [below for nested schema](#nestedatt--cert_list))

<a id="nestedatt--cert_list"></a>
### Nested Schema for `cert_list`

Read-Only:

- `certificate_id` (String) Certificate ID
- `name` (String) The name of certificate