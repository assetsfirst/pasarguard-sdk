# SetupApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createOwner**](#createowner) | **POST** /api/setup/owner | Create Owner|
|[**deleteOwner**](#deleteowner) | **DELETE** /api/setup/owner | Delete Owner|
|[**resetOwnerPassword**](#resetownerpassword) | **PATCH** /api/setup/owner | Reset Owner Password|
|[**upgradeOwner**](#upgradeowner) | **POST** /api/setup/owner/upgrade | Upgrade Owner|

# **createOwner**
> AdminDetails createOwner(ownerCreateRequest)

Create the owner admin using a one-time temp key.

### Example

```typescript
import {
    SetupApi,
    Configuration,
    OwnerCreateRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new SetupApi(configuration);

let ownerCreateRequest: OwnerCreateRequest; //

const { status, data } = await apiInstance.createOwner(
    ownerCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ownerCreateRequest** | **OwnerCreateRequest**|  | |


### Return type

**AdminDetails**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**409** | Conflict Error |  -  |
|**410** | Key already used or expired |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteOwner**
> deleteOwner()

Delete the owner admin using a one-time temp key.

### Example

```typescript
import {
    SetupApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SetupApi(configuration);

let key: string; //One-time temp key for deleting the owner admin (default to undefined)

const { status, data } = await apiInstance.deleteOwner(
    key
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **key** | [**string**] | One-time temp key for deleting the owner admin | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**404** | NotFound Error |  -  |
|**410** | Key already used or expired |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetOwnerPassword**
> AdminDetails resetOwnerPassword(ownerResetRequest)

Reset the owner admin\'s password using a one-time temp key.

### Example

```typescript
import {
    SetupApi,
    Configuration,
    OwnerResetRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new SetupApi(configuration);

let ownerResetRequest: OwnerResetRequest; //

const { status, data } = await apiInstance.resetOwnerPassword(
    ownerResetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ownerResetRequest** | **OwnerResetRequest**|  | |


### Return type

**AdminDetails**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**404** | NotFound Error |  -  |
|**410** | Key already used or expired |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upgradeOwner**
> AdminDetails upgradeOwner(ownerUpgradeRequest)

Upgrade an existing admin to owner using a one-time temp key.

### Example

```typescript
import {
    SetupApi,
    Configuration,
    OwnerUpgradeRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new SetupApi(configuration);

let ownerUpgradeRequest: OwnerUpgradeRequest; //

const { status, data } = await apiInstance.upgradeOwner(
    ownerUpgradeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ownerUpgradeRequest** | **OwnerUpgradeRequest**|  | |


### Return type

**AdminDetails**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**404** | NotFound Error |  -  |
|**409** | Conflict Error |  -  |
|**410** | Key already used or expired |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

