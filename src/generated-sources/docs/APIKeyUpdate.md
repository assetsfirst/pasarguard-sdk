# APIKeyUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**admin_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**permissions** | [**RolePermissions**](RolePermissions.md) |  | [optional] [default to undefined]
**inherit_permissions** | **boolean** |  | [optional] [default to undefined]
**expire_date** | **string** |  | [optional] [default to undefined]
**status** | [**APIKeyStatus**](APIKeyStatus.md) |  | [optional] [default to undefined]

## Example

```typescript
import { APIKeyUpdate } from './api';

const instance: APIKeyUpdate = {
    admin_id,
    name,
    note,
    permissions,
    inherit_permissions,
    expire_date,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
