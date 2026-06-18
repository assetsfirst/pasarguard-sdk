# AdminDetails

Complete admin model with all fields for database representation and API responses.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**username** | **string** |  | [default to undefined]
**telegram_id** | **number** |  | [optional] [default to undefined]
**discord_webhook** | **string** |  | [optional] [default to undefined]
**sub_domain** | **string** |  | [optional] [default to undefined]
**profile_title** | **string** |  | [optional] [default to undefined]
**support_url** | **string** |  | [optional] [default to undefined]
**notification_enable** | [**UserNotificationEnable**](UserNotificationEnable.md) |  | [optional] [default to undefined]
**total_users** | **number** |  | [optional] [default to 0]
**used_traffic** | **number** |  | [optional] [default to 0]
**data_limit** | **number** |  | [optional] [default to undefined]
**status** | [**AdminStatus**](AdminStatus.md) |  | [optional] [default to undefined]
**sub_template** | **string** |  | [optional] [default to undefined]
**lifetime_used_traffic** | **number** |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**role** | [**AdminRoleData**](AdminRoleData.md) |  | [optional] [default to undefined]
**permission_overrides** | [**RoleLimits**](RoleLimits.md) |  | [optional] [default to undefined]
**is_disabled** | **boolean** |  | [readonly] [default to undefined]
**is_limited** | **boolean** |  | [readonly] [default to undefined]

## Example

```typescript
import { AdminDetails } from './api';

const instance: AdminDetails = {
    id,
    username,
    telegram_id,
    discord_webhook,
    sub_domain,
    profile_title,
    support_url,
    notification_enable,
    total_users,
    used_traffic,
    data_limit,
    status,
    sub_template,
    lifetime_used_traffic,
    note,
    role,
    permission_overrides,
    is_disabled,
    is_limited,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
