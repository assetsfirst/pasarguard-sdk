# APIKeysApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bulkDeleteApiKeys**](#bulkdeleteapikeys) | **POST** /api/api_keys/bulk/delete | Bulk Delete Api Keys|
|[**createApiKey**](#createapikey) | **POST** /api/api_key | Create Api Key|
|[**getApiKey**](#getapikey) | **GET** /api/api_key/{key_id} | Get Api Key|
|[**listApiKeys**](#listapikeys) | **GET** /api/api_keys | List Api Keys|
|[**modifyApiKey**](#modifyapikey) | **PATCH** /api/api_key/{key_id} | Modify Api Key|
|[**removeApiKey**](#removeapikey) | **DELETE** /api/api_key/{key_id} | Remove Api Key|
|[**revokeApiKey**](#revokeapikey) | **POST** /api/api_key/{key_id}/revoke | Revoke Api Key|

# **bulkDeleteApiKeys**
> RemoveAPIKeysResponse bulkDeleteApiKeys(bulkAPIKeySelection)


### Example

```typescript
import {
    APIKeysApi,
    Configuration,
    BulkAPIKeySelection
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let bulkAPIKeySelection: BulkAPIKeySelection; //

const { status, data } = await apiInstance.bulkDeleteApiKeys(
    bulkAPIKeySelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAPIKeySelection** | **BulkAPIKeySelection**|  | |


### Return type

**RemoveAPIKeysResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**400** | BadRequest Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createApiKey**
> APIKeyCreateResponse createApiKey(aPIKeyCreate)


### Example

```typescript
import {
    APIKeysApi,
    Configuration,
    APIKeyCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let aPIKeyCreate: APIKeyCreate; //

const { status, data } = await apiInstance.createApiKey(
    aPIKeyCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **aPIKeyCreate** | **APIKeyCreate**|  | |


### Return type

**APIKeyCreateResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getApiKey**
> APIKeyResponse getApiKey()


### Example

```typescript
import {
    APIKeysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let keyId: number; // (default to undefined)

const { status, data } = await apiInstance.getApiKey(
    keyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **keyId** | [**number**] |  | defaults to undefined|


### Return type

**APIKeyResponse**

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

# **listApiKeys**
> APIKeysResponse listApiKeys()


### Example

```typescript
import {
    APIKeysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let keyId: number; // (optional) (default to undefined)
let name: string; // (optional) (default to undefined)
let status: APIKeyStatus; // (optional) (default to undefined)

const { status, data } = await apiInstance.listApiKeys(
    offset,
    limit,
    keyId,
    name,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **keyId** | [**number**] |  | (optional) defaults to undefined|
| **name** | [**string**] |  | (optional) defaults to undefined|
| **status** | **APIKeyStatus** |  | (optional) defaults to undefined|


### Return type

**APIKeysResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyApiKey**
> APIKeyResponse modifyApiKey(aPIKeyUpdate)


### Example

```typescript
import {
    APIKeysApi,
    Configuration,
    APIKeyUpdate
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let keyId: number; // (default to undefined)
let aPIKeyUpdate: APIKeyUpdate; //

const { status, data } = await apiInstance.modifyApiKey(
    keyId,
    aPIKeyUpdate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **aPIKeyUpdate** | **APIKeyUpdate**|  | |
| **keyId** | [**number**] |  | defaults to undefined|


### Return type

**APIKeyResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeApiKey**
> removeApiKey()


### Example

```typescript
import {
    APIKeysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let keyId: number; // (default to undefined)

const { status, data } = await apiInstance.removeApiKey(
    keyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **keyId** | [**number**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **revokeApiKey**
> APIKeyCreateResponse revokeApiKey()


### Example

```typescript
import {
    APIKeysApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new APIKeysApi(configuration);

let keyId: number; // (default to undefined)

const { status, data } = await apiInstance.revokeApiKey(
    keyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **keyId** | [**number**] |  | defaults to undefined|


### Return type

**APIKeyCreateResponse**

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

