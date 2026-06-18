# RolePermissions

Typed permission map. Missing resource or action = denied. Each action value is True (allowed), {\"scope\": N} (scoped), or None (denied).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**UsersPermissions**](UsersPermissions.md) |  | [optional] [default to undefined]
**admins** | [**AdminsPermissions**](AdminsPermissions.md) |  | [optional] [default to undefined]
**nodes** | [**NodesPermissions**](NodesPermissions.md) |  | [optional] [default to undefined]
**groups** | [**CRUDPermissions**](CRUDPermissions.md) |  | [optional] [default to undefined]
**hosts** | [**HostsPermissions**](HostsPermissions.md) |  | [optional] [default to undefined]
**templates** | [**CRUDPermissions**](CRUDPermissions.md) |  | [optional] [default to undefined]
**client_templates** | [**CRUDPermissions**](CRUDPermissions.md) |  | [optional] [default to undefined]
**cores** | [**CRUDPermissions**](CRUDPermissions.md) |  | [optional] [default to undefined]
**settings** | [**SettingsPermissions**](SettingsPermissions.md) |  | [optional] [default to undefined]
**system** | [**SystemPermissions**](SystemPermissions.md) |  | [optional] [default to undefined]
**hwids** | [**HwidsPermissions**](HwidsPermissions.md) |  | [optional] [default to undefined]
**admin_roles** | [**CRUDPermissions**](CRUDPermissions.md) |  | [optional] [default to undefined]

## Example

```typescript
import { RolePermissions } from './api';

const instance: RolePermissions = {
    users,
    admins,
    nodes,
    groups,
    hosts,
    templates,
    client_templates,
    cores,
    settings,
    system,
    hwids,
    admin_roles,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
