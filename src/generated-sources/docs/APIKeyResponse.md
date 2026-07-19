# APIKeyResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**permissions** | [**RolePermissions**](RolePermissions.md) |  | [optional] [default to undefined]
**inherit_permissions** | **boolean** |  | [optional] [default to true]
**expire_date** | **string** |  | [optional] [default to undefined]
**id** | **number** |  | [default to undefined]
**admin_id** | **number** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**api_key_trimmed** | **string** |  | [default to undefined]
**revoked_at** | **string** |  | [optional] [default to undefined]
**status** | [**APIKeyStatus**](APIKeyStatus.md) |  | [optional] [default to undefined]
**is_expired** | **boolean** |  | [optional] [default to false]

## Example

```typescript
import { APIKeyResponse } from './api';

const instance: APIKeyResponse = {
    name,
    note,
    permissions,
    inherit_permissions,
    expire_date,
    id,
    admin_id,
    created_at,
    api_key_trimmed,
    revoked_at,
    status,
    is_expired,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
