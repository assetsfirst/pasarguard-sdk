# RoleLimits


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**max_users** | **number** |  | [optional] [default to undefined]
**data_limit_min** | **number** |  | [optional] [default to undefined]
**data_limit_max** | **number** |  | [optional] [default to undefined]
**expire_min** | **number** |  | [optional] [default to undefined]
**expire_max** | **number** |  | [optional] [default to undefined]
**min_hwid_per_user** | **number** |  | [optional] [default to undefined]
**max_hwid_per_user** | **number** |  | [optional] [default to undefined]
**on_hold_timeout_min** | **number** |  | [optional] [default to undefined]
**on_hold_timeout_max** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { RoleLimits } from './api';

const instance: RoleLimits = {
    max_users,
    data_limit_min,
    data_limit_max,
    expire_min,
    expire_max,
    min_hwid_per_user,
    max_hwid_per_user,
    on_hold_timeout_min,
    on_hold_timeout_max,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
