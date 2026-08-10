# RoleHWIDSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **boolean** |  | [optional] [default to true]
**forced** | **boolean** |  | [optional] [default to false]
**require_hwid_for_manual_sub** | **boolean** |  | [optional] [default to false]
**fallback_limit** | **number** |  | [optional] [default to undefined]
**min_limit** | **number** |  | [optional] [default to undefined]
**max_limit** | **number** |  | [optional] [default to undefined]
**mode** | [**HWIDMode**](HWIDMode.md) |  | [optional] [default to undefined]

## Example

```typescript
import { RoleHWIDSettings } from './api';

const instance: RoleHWIDSettings = {
    enabled,
    forced,
    require_hwid_for_manual_sub,
    fallback_limit,
    min_limit,
    max_limit,
    mode,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
