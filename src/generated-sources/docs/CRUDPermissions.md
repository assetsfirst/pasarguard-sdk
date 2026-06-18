# CRUDPermissions

Standard create/read/read_simple/update/delete permissions. Used directly by: groups, templates, client_templates, cores, admin_roles. Also serves as base for resources with additional actions.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | [**Create**](Create.md) |  | [optional] [default to undefined]
**read** | [**Read**](Read.md) |  | [optional] [default to undefined]
**read_simple** | [**ReadSimple**](ReadSimple.md) |  | [optional] [default to undefined]
**update** | [**Update**](Update.md) |  | [optional] [default to undefined]
**_delete** | [**Delete**](Delete.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CRUDPermissions } from './api';

const instance: CRUDPermissions = {
    create,
    read,
    read_simple,
    update,
    _delete,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
