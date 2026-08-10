# BulkUsersFromTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_template_id** | **number** |  | [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**username** | **string** |  | [optional] [default to undefined]
**count** | **number** |  | [default to undefined]
**strategy** | [**UsernameGenerationStrategy**](UsernameGenerationStrategy.md) |  | [optional] [default to undefined]
**start_number** | **number** | Starting suffix for sequence strategy (defaults to 1; base username digits are ignored) | [optional] [default to undefined]

## Example

```typescript
import { BulkUsersFromTemplate } from './api';

const instance: BulkUsersFromTemplate = {
    user_template_id,
    note,
    username,
    count,
    strategy,
    start_number,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
