---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "datadog_rum_application Resource - terraform-provider-datadog"
subcategory: ""
description: |-
  Provides a Datadog RUM application resource. This can be used to create and manage Datadog RUM applications.
---

# datadog_rum_application (Resource)

Provides a Datadog RUM application resource. This can be used to create and manage Datadog RUM applications.

## Example Usage

```terraform
resource "datadog_rum_application" "rum_application" {
  name = "my-application"
  type = "browser"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The name of the RUM application

### Optional

- `type` (String) The RUM application type. Supported values are `browser`, `ios`, `android`, `react-native`, `flutter`

### Read-Only

- `client_token` (String) The client token
- `id` (String) The ID of this resource.

## Import

Import is supported using the following syntax:

```shell
terraform import datadog_rum_application.rum_application a1b2c3d4-a1b2-a1b2-a1b2-a1b2c3d4e5f6
```