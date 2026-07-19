# APIKeyCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**permissions** | [**RolePermissions**](RolePermissions.md) |  | [optional] [default to undefined]
**inherit_permissions** | **boolean** |  | [optional] [default to true]
**expire_date** | **string** |  | [optional] [default to undefined]
**admin_id** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { APIKeyCreate } from './api';

const instance: APIKeyCreate = {
    name,
    note,
    permissions,
    inherit_permissions,
    expire_date,
    admin_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
