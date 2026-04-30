# BulkUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **number** |  | [default to undefined]
**dry_run** | **boolean** |  | [optional] [default to false]
**group_ids** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**admins** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**users** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**status** | [**Set&lt;UserStatus&gt;**](UserStatus.md) |  | [optional] [default to undefined]
**expired_after** | **string** |  | [optional] [default to undefined]
**expired_before** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { BulkUser } from './api';

const instance: BulkUser = {
    amount,
    dry_run,
    group_ids,
    admins,
    users,
    status,
    expired_after,
    expired_before,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
