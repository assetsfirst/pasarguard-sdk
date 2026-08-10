# FinalMaskQuicParams


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**congestion** | [**FinalMaskQuicCongestion**](FinalMaskQuicCongestion.md) |  | [optional] [default to undefined]
**debug** | **boolean** |  | [optional] [default to undefined]
**bbrProfile** | **string** |  | [optional] [default to undefined]
**brutalUp** | [**Brutalup**](Brutalup.md) |  | [optional] [default to undefined]
**brutalDown** | [**Brutaldown**](Brutaldown.md) |  | [optional] [default to undefined]
**udpHop** | [**FinalMaskUdpHop**](FinalMaskUdpHop.md) |  | [optional] [default to undefined]
**initStreamReceiveWindow** | **number** |  | [optional] [default to undefined]
**maxStreamReceiveWindow** | **number** |  | [optional] [default to undefined]
**initConnectionReceiveWindow** | **number** |  | [optional] [default to undefined]
**maxConnectionReceiveWindow** | **number** |  | [optional] [default to undefined]
**maxIdleTimeout** | **number** |  | [optional] [default to undefined]
**keepAlivePeriod** | **number** |  | [optional] [default to undefined]
**disablePathMTUDiscovery** | **boolean** |  | [optional] [default to undefined]
**maxIncomingStreams** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { FinalMaskQuicParams } from './api';

const instance: FinalMaskQuicParams = {
    congestion,
    debug,
    bbrProfile,
    brutalUp,
    brutalDown,
    udpHop,
    initStreamReceiveWindow,
    maxStreamReceiveWindow,
    initConnectionReceiveWindow,
    maxConnectionReceiveWindow,
    maxIdleTimeout,
    keepAlivePeriod,
    disablePathMTUDiscovery,
    maxIncomingStreams,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
