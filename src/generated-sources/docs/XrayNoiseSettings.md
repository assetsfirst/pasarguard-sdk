# XrayNoiseSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **string** |  | [default to undefined]
**packet** | [**Packet**](Packet.md) |  | [optional] [default to undefined]
**delay** | [**Delay**](Delay.md) |  | [optional] [default to undefined]
**apply_to** | **string** |  | [optional] [default to 'ip']
**rand** | [**Rand**](Rand.md) |  | [optional] [default to undefined]
**randRange** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { XrayNoiseSettings } from './api';

const instance: XrayNoiseSettings = {
    type,
    packet,
    delay,
    apply_to,
    rand,
    randRange,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
