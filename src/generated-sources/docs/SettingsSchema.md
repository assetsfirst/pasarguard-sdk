# SettingsSchema


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**telegram** | [**Telegram**](Telegram.md) |  | [optional] [default to undefined]
**webhook** | [**Webhook**](Webhook.md) |  | [optional] [default to undefined]
**notification_settings** | [**NotificationSettings**](NotificationSettings.md) |  | [optional] [default to undefined]
**notification_enable** | [**NotificationEnable**](NotificationEnable.md) |  | [optional] [default to undefined]
**subscription** | [**Subscription**](Subscription.md) |  | [optional] [default to undefined]
**hwid** | [**HWIDSettings**](HWIDSettings.md) |  | [optional] [default to undefined]
**general** | [**General**](General.md) |  | [optional] [default to undefined]

## Example

```typescript
import { SettingsSchema } from './api';

const instance: SettingsSchema = {
    telegram,
    webhook,
    notification_settings,
    notification_enable,
    subscription,
    hwid,
    general,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
