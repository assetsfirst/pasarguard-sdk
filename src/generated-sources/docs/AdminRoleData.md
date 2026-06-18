# AdminRoleData

Runtime role data carried on AdminDetails — only the fields needed for permission checks.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to '']
**is_owner** | **boolean** |  | [optional] [default to false]
**permissions** | [**RolePermissions**](RolePermissions.md) |  | [optional] [default to undefined]
**limits** | [**RoleLimits**](RoleLimits.md) |  | [optional] [default to undefined]
**features** | [**RoleFeatures**](RoleFeatures.md) |  | [optional] [default to undefined]
**access** | [**RoleAccess**](RoleAccess.md) |  | [optional] [default to undefined]
**hwid** | [**RoleHWIDSettings**](RoleHWIDSettings.md) |  | [optional] [default to undefined]
**disabled_when_limited** | **boolean** |  | [optional] [default to false]
**disconnect_users_when_limited** | **boolean** |  | [optional] [default to true]
**disconnect_users_when_disabled** | **boolean** |  | [optional] [default to true]

## Example

```typescript
import { AdminRoleData } from './api';

const instance: AdminRoleData = {
    id,
    name,
    is_owner,
    permissions,
    limits,
    features,
    access,
    hwid,
    disabled_when_limited,
    disconnect_users_when_limited,
    disconnect_users_when_disabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
