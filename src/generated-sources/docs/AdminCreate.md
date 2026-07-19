# AdminCreate

Model for creating new admin accounts requiring username and password.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**password** | **string** |  | [default to undefined]
**telegram_id** | **number** |  | [optional] [default to undefined]
**discord_webhook** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**data_limit** | **number** |  | [optional] [default to undefined]
**sub_template** | **string** |  | [optional] [default to undefined]
**sub_domain** | **string** |  | [optional] [default to undefined]
**profile_title** | **string** |  | [optional] [default to undefined]
**support_url** | **string** |  | [optional] [default to undefined]
**custom_variables** | [**Array&lt;CustomVariable&gt;**](CustomVariable.md) |  | [optional] [default to undefined]
**note** | **string** |  | [optional] [default to undefined]
**notification_enable** | [**UserNotificationEnable**](UserNotificationEnable.md) |  | [optional] [default to undefined]
**role_id** | **number** |  | [default to undefined]
**permission_overrides** | [**RoleLimits**](RoleLimits.md) |  | [optional] [default to undefined]
**username** | **string** |  | [default to undefined]

## Example

```typescript
import { AdminCreate } from './api';

const instance: AdminCreate = {
    password,
    telegram_id,
    discord_webhook,
    status,
    data_limit,
    sub_template,
    sub_domain,
    profile_title,
    support_url,
    custom_variables,
    note,
    notification_enable,
    role_id,
    permission_overrides,
    username,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
