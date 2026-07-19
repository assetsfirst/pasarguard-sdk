# FinalMaskInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tcp** | [**Array&lt;FinalMaskTcpLayerInput&gt;**](FinalMaskTcpLayerInput.md) |  | [optional] [default to undefined]
**udp** | [**Array&lt;FinalMaskUdpLayer&gt;**](FinalMaskUdpLayer.md) |  | [optional] [default to undefined]
**quicParams** | [**FinalMaskQuicParams**](FinalMaskQuicParams.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FinalMaskInput } from './api';

const instance: FinalMaskInput = {
    tcp,
    udp,
    quicParams,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
