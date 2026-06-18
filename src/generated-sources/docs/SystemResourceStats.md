# SystemResourceStats


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **string** |  | [default to undefined]
**uptime_seconds** | **number** |  | [default to undefined]
**mem_total** | **number** |  | [optional] [default to undefined]
**mem_used** | **number** |  | [optional] [default to undefined]
**disk_total** | **number** |  | [optional] [default to undefined]
**disk_used** | **number** |  | [optional] [default to undefined]
**cpu_cores** | **number** |  | [optional] [default to undefined]
**cpu_usage** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { SystemResourceStats } from './api';

const instance: SystemResourceStats = {
    version,
    uptime_seconds,
    mem_total,
    mem_used,
    disk_total,
    disk_used,
    cpu_cores,
    cpu_usage,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
