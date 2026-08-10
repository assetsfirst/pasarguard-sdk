# Settings1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client** | [**Array&lt;XrayNoiseSettings&gt;**](XrayNoiseSettings.md) |  | [optional] [default to undefined]
**server** | [**Array&lt;XrayNoiseSettings&gt;**](XrayNoiseSettings.md) |  | [optional] [default to undefined]
**password** | **string** |  | [optional] [default to undefined]
**ascii** | **string** |  | [optional] [default to undefined]
**customTable** | **string** |  | [optional] [default to undefined]
**customTables** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**paddingMin** | **number** |  | [optional] [default to undefined]
**paddingMax** | **number** |  | [optional] [default to undefined]
**domain** | **string** |  | [optional] [default to undefined]
**domains** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**resolvers** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**dgram** | **boolean** |  | [optional] [default to undefined]
**ips** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**listenIp** | **string** |  | [optional] [default to undefined]
**id** | **number** |  | [optional] [default to undefined]
**reset** | [**Reset**](Reset.md) |  | [optional] [default to undefined]
**noise** | [**Array&lt;XrayNoiseSettings&gt;**](XrayNoiseSettings.md) |  | [optional] [default to undefined]
**packetSize** | [****](.md) |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**stunServers** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**tlsConfig** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**header** | **string** |  | [optional] [default to undefined]
**value** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Settings1 } from './api';

const instance: Settings1 = {
    client,
    server,
    password,
    ascii,
    customTable,
    customTables,
    paddingMin,
    paddingMax,
    domain,
    domains,
    resolvers,
    dgram,
    ips,
    listenIp,
    id,
    reset,
    noise,
    packetSize,
    url,
    stunServers,
    tlsConfig,
    header,
    value,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
