# RealityScanRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target** | **string** | host or host:port to probe (port defaults to 443) | [default to undefined]
**timeout** | **number** | Per-probe timeout in seconds (1-20, default 10) | [optional] [default to undefined]

## Example

```typescript
import { RealityScanRequest } from './api';

const instance: RealityScanRequest = {
    target,
    timeout,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
