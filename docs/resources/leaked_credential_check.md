---
page_title: "cloudflare_leaked_credential_check Resource - Cloudflare"
subcategory: ""
description: |-
  Provides a Cloudflare Leaked Credential Check resource to be used for managing the status of the Cloudflare Leaked Credential detection within a specific zone.
---

# cloudflare_leaked_credential_check (Resource)

Provides a Cloudflare Leaked Credential Check resource to be used for managing the status of the Cloudflare Leaked Credential detection within a specific zone.

## Example Usage

```terraform
# Enable the Leaked Credentials Check detection
resource "cloudflare_leaked_credential_check" "example" {
    zone_id = "399c6f4950c01a5a141b99ff7fbcbd8b"
    enabled = true
}
```
<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `enabled` (Boolean) State of the Leaked Credential Check detection
- `zone_id` (String) The zone identifier to target for the resource.

## Import

Import is supported using the following syntax:

```shell
terraform import cloudflare_leaked_credential_check.example <zone_id>
```
