# BulkUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dry_run** | **boolean** |  | [optional] [default to false]
**group_ids** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**admins** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**users** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**status** | [**Set&lt;UserStatus&gt;**](UserStatus.md) |  | [optional] [default to undefined]
**expire_after** | **string** |  | [optional] [default to undefined]
**expire_before** | **string** |  | [optional] [default to undefined]
**amount** | **number** |  | [default to undefined]

## Example

```typescript
import { BulkUser } from './api';

const instance: BulkUser = {
    dry_run,
    group_ids,
    admins,
    users,
    status,
    expire_after,
    expire_before,
    amount,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
