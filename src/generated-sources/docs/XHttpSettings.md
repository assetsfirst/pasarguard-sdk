# XHttpSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mode** | [**XHttpModes**](XHttpModes.md) |  | [optional] [default to undefined]
**no_grpc_header** | **boolean** |  | [optional] [default to undefined]
**x_padding_bytes** | **string** |  | [optional] [default to undefined]
**x_padding_obfs_mode** | **boolean** |  | [optional] [default to undefined]
**x_padding_key** | **string** |  | [optional] [default to undefined]
**x_padding_header** | **string** |  | [optional] [default to undefined]
**x_padding_placement** | **string** |  | [optional] [default to undefined]
**x_padding_method** | **string** |  | [optional] [default to undefined]
**uplink_http_method** | **string** |  | [optional] [default to undefined]
**session_placement** | **string** |  | [optional] [default to undefined]
**session_key** | **string** |  | [optional] [default to undefined]
**session_id_table** | **string** |  | [optional] [default to undefined]
**session_id_length** | **string** |  | [optional] [default to undefined]
**seq_placement** | **string** |  | [optional] [default to undefined]
**seq_key** | **string** |  | [optional] [default to undefined]
**uplink_data_placement** | **string** |  | [optional] [default to undefined]
**uplink_data_key** | **string** |  | [optional] [default to undefined]
**uplink_chunk_size** | **string** |  | [optional] [default to undefined]
**sc_max_each_post_bytes** | **string** |  | [optional] [default to undefined]
**sc_min_posts_interval_ms** | **string** |  | [optional] [default to undefined]
**xmux** | [**XMuxSettings**](XMuxSettings.md) |  | [optional] [default to undefined]
**download_settings** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { XHttpSettings } from './api';

const instance: XHttpSettings = {
    mode,
    no_grpc_header,
    x_padding_bytes,
    x_padding_obfs_mode,
    x_padding_key,
    x_padding_header,
    x_padding_placement,
    x_padding_method,
    uplink_http_method,
    session_placement,
    session_key,
    session_id_table,
    session_id_length,
    seq_placement,
    seq_key,
    uplink_data_placement,
    uplink_data_key,
    uplink_chunk_size,
    sc_max_each_post_bytes,
    sc_min_posts_interval_ms,
    xmux,
    download_settings,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
