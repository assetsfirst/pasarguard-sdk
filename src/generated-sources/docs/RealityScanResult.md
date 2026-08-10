# RealityScanResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target** | **string** |  | [default to undefined]
**host** | **string** |  | [default to undefined]
**ip** | **string** |  | [optional] [default to undefined]
**port** | **number** |  | [default to undefined]
**sni** | **string** |  | [optional] [default to undefined]
**sni_discovered** | **boolean** |  | [optional] [default to false]
**feasible** | **boolean** |  | [default to undefined]
**tls13** | **boolean** |  | [default to undefined]
**tls_version** | **string** |  | [optional] [default to undefined]
**h2** | **boolean** |  | [default to undefined]
**alpn** | **string** |  | [optional] [default to undefined]
**x25519** | **boolean** |  | [optional] [default to undefined]
**post_quantum** | **boolean** |  | [optional] [default to undefined]
**curve** | **string** |  | [optional] [default to undefined]
**h3** | **boolean** |  | [optional] [default to false]
**cert_valid** | **boolean** |  | [default to undefined]
**cert_subject** | **string** |  | [optional] [default to undefined]
**cert_issuer** | **string** |  | [optional] [default to undefined]
**not_after** | **string** |  | [optional] [default to undefined]
**server_names** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**latency_ms** | **number** |  | [optional] [default to undefined]
**reason** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { RealityScanResult } from './api';

const instance: RealityScanResult = {
    target,
    host,
    ip,
    port,
    sni,
    sni_discovered,
    feasible,
    tls13,
    tls_version,
    h2,
    alpn,
    x25519,
    post_quantum,
    curve,
    h3,
    cert_valid,
    cert_subject,
    cert_issuer,
    not_after,
    server_names,
    latency_ms,
    reason,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
