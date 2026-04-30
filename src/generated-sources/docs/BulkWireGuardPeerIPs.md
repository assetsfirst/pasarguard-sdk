# BulkWireGuardPeerIPs

Re-seat WireGuard peer IPs (same scoping as BulkUser: users, admins, group_ids, status).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**confirm** | **boolean** |  | [optional] [default to false]
**dry_run** | **boolean** |  | [optional] [default to false]
**replace_all** | **boolean** |  | [optional] [default to false]
**group_ids** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**admins** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**users** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**status** | [**Set&lt;UserStatus&gt;**](UserStatus.md) |  | [optional] [default to undefined]

## Example

```typescript
import { BulkWireGuardPeerIPs } from './api';

const instance: BulkWireGuardPeerIPs = {
    confirm,
    dry_run,
    replace_all,
    group_ids,
    admins,
    users,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
