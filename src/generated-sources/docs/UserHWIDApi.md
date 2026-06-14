# UserHWIDApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteUserHwid**](#deleteuserhwid) | **DELETE** /api/user/{user_id}/hwids/{hwid} | Delete User Hwid|
|[**getUserHwids**](#getuserhwids) | **GET** /api/user/{user_id}/hwids | Get User Hwids|
|[**resetUserHwids**](#resetuserhwids) | **POST** /api/user/{user_id}/hwids/reset | Reset User Hwids|

# **deleteUserHwid**
> any deleteUserHwid()

Delete a specific hardware ID from user

### Example

```typescript
import {
    UserHWIDApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserHWIDApi(configuration);

let userId: number; // (default to undefined)
let hwid: string; // (default to undefined)

const { status, data } = await apiInstance.deleteUserHwid(
    userId,
    hwid
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|
| **hwid** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserHwids**
> UserHWIDListResponse getUserHwids()

Get user\'s registered hardware IDs

### Example

```typescript
import {
    UserHWIDApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserHWIDApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.getUserHwids(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserHWIDListResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetUserHwids**
> any resetUserHwids()

Delete all hardware IDs for user

### Example

```typescript
import {
    UserHWIDApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserHWIDApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.resetUserHwids(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

