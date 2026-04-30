# WireGuardHostOverrides

Optional per-host values merged into WireGuard subscription output.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allowed_ips** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**mtu** | **number** |  | [optional] [default to undefined]
**reserved** | **string** |  | [optional] [default to undefined]
**keepalive_seconds** | **number** |  | [optional] [default to undefined]
**dns** | **Array&lt;string&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { WireGuardHostOverrides } from './api';

const instance: WireGuardHostOverrides = {
    allowed_ips,
    mtu,
    reserved,
    keepalive_seconds,
    dns,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
