# UserCountMetricStatsList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**period** | [**Period**](Period.md) |  | [optional] [default to undefined]
**start** | **string** |  | [default to undefined]
**end** | **string** |  | [default to undefined]
**metric** | [**UserCountMetric**](UserCountMetric.md) |  | [default to undefined]
**count_during_period** | **number** |  | [optional] [default to 0]
**stats** | **{ [key: string]: Array&lt;UserCountMetricStat&gt;; }** |  | [default to undefined]

## Example

```typescript
import { UserCountMetricStatsList } from './api';

const instance: UserCountMetricStatsList = {
    period,
    start,
    end,
    metric,
    count_during_period,
    stats,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
