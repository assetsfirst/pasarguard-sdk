# AdminNotificationEnable


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create** | **boolean** |  | [optional] [default to true]
**modify** | **boolean** |  | [optional] [default to true]
**_delete** | **boolean** |  | [optional] [default to true]
**reset_usage** | **boolean** |  | [optional] [default to true]
**login** | **boolean** |  | [optional] [default to true]
**usage_limit_warning** | **boolean** |  | [optional] [default to true]
**usage_limit_warning_percentages** | **Array&lt;number&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { AdminNotificationEnable } from './api';

const instance: AdminNotificationEnable = {
    create,
    modify,
    _delete,
    reset_usage,
    login,
    usage_limit_warning,
    usage_limit_warning_percentages,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
