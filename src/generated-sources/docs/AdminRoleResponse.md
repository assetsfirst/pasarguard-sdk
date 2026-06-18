# AdminRoleResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**permissions** | [**RolePermissions**](RolePermissions.md) |  | [optional] [default to undefined]
**limits** | [**RoleLimits**](RoleLimits.md) |  | [optional] [default to undefined]
**features** | [**RoleFeatures**](RoleFeatures.md) |  | [optional] [default to undefined]
**access** | [**RoleAccess**](RoleAccess.md) |  | [optional] [default to undefined]
**hwid** | [**RoleHWIDSettings**](RoleHWIDSettings.md) |  | [optional] [default to undefined]
**disabled_when_limited** | **boolean** |  | [optional] [default to false]
**disconnect_users_when_limited** | **boolean** |  | [optional] [default to true]
**disconnect_users_when_disabled** | **boolean** |  | [optional] [default to true]
**id** | **number** |  | [default to undefined]
**is_owner** | **boolean** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]

## Example

```typescript
import { AdminRoleResponse } from './api';

const instance: AdminRoleResponse = {
    name,
    permissions,
    limits,
    features,
    access,
    hwid,
    disabled_when_limited,
    disconnect_users_when_limited,
    disconnect_users_when_disabled,
    id,
    is_owner,
    created_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
