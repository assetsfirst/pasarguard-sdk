# Settings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clients** | **Array&lt;Array&lt;XrayNoiseSettings&gt;&gt;** |  | [optional] [default to undefined]
**servers** | **Array&lt;Array&lt;XrayNoiseSettings&gt;&gt;** |  | [optional] [default to undefined]
**errors** | **Array&lt;Array&lt;XrayNoiseSettings&gt;&gt;** |  | [optional] [default to undefined]
**packets** | **string** |  | [optional] [default to undefined]
**lengths** | [**Array&lt;FinalMaskFragmentSettingsLengthsInner&gt;**](FinalMaskFragmentSettingsLengthsInner.md) |  | [optional] [default to undefined]
**delays** | [**Array&lt;FinalMaskFragmentSettingsLengthsInner&gt;**](FinalMaskFragmentSettingsLengthsInner.md) |  | [optional] [default to undefined]
**maxSplit** | [**Maxsplit**](Maxsplit.md) |  | [optional] [default to undefined]
**password** | **string** |  | [optional] [default to undefined]
**ascii** | **string** |  | [optional] [default to undefined]
**customTable** | **string** |  | [optional] [default to undefined]
**customTables** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**paddingMin** | **number** |  | [optional] [default to undefined]
**paddingMax** | **number** |  | [optional] [default to undefined]
**hostname** | **string** |  | [optional] [default to undefined]
**profiles** | [**Array&lt;FinalMaskXmcProfile&gt;**](FinalMaskXmcProfile.md) |  | [optional] [default to undefined]
**usernames** | **Array&lt;string&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { Settings } from './api';

const instance: Settings = {
    clients,
    servers,
    errors,
    packets,
    lengths,
    delays,
    maxSplit,
    password,
    ascii,
    customTable,
    customTables,
    paddingMin,
    paddingMax,
    hostname,
    profiles,
    usernames,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
