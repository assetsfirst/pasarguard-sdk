# FinalMaskOutput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tcp** | [**Array&lt;FinalMaskTcpLayerOutput&gt;**](FinalMaskTcpLayerOutput.md) |  | [optional] [default to undefined]
**udp** | [**Array&lt;FinalMaskUdpLayer&gt;**](FinalMaskUdpLayer.md) |  | [optional] [default to undefined]
**quicParams** | [**FinalMaskQuicParams**](FinalMaskQuicParams.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FinalMaskOutput } from './api';

const instance: FinalMaskOutput = {
    tcp,
    udp,
    quicParams,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
