# ClientTemplateApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bulkDeleteClientTemplates**](#bulkdeleteclienttemplates) | **POST** /api/client_templates/bulk/delete | Bulk Delete Client Templates|
|[**createClientTemplate**](#createclienttemplate) | **POST** /api/client_template | Create Client Template|
|[**getClientTemplate**](#getclienttemplate) | **GET** /api/client_template/{template_id} | Get Client Template|
|[**getClientTemplates**](#getclienttemplates) | **GET** /api/client_templates | Get Client Templates|
|[**getClientTemplatesSimple**](#getclienttemplatessimple) | **GET** /api/client_templates/simple | Get Client Templates Simple|
|[**modifyClientTemplate**](#modifyclienttemplate) | **PUT** /api/client_template/{template_id} | Modify Client Template|
|[**removeClientTemplate**](#removeclienttemplate) | **DELETE** /api/client_template/{template_id} | Remove Client Template|

# **bulkDeleteClientTemplates**
> RemoveClientTemplatesResponse bulkDeleteClientTemplates(bulkClientTemplateSelection)

Delete selected client templates by ID.

### Example

```typescript
import {
    ClientTemplateApi,
    Configuration,
    BulkClientTemplateSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let bulkClientTemplateSelection: BulkClientTemplateSelection; //

const { status, data } = await apiInstance.bulkDeleteClientTemplates(
    bulkClientTemplateSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkClientTemplateSelection** | **BulkClientTemplateSelection**|  | |


### Return type

**RemoveClientTemplatesResponse**

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

# **createClientTemplate**
> ClientTemplateResponse createClientTemplate(clientTemplateCreate)


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration,
    ClientTemplateCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let clientTemplateCreate: ClientTemplateCreate; //

const { status, data } = await apiInstance.createClientTemplate(
    clientTemplateCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **clientTemplateCreate** | **ClientTemplateCreate**|  | |


### Return type

**ClientTemplateResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getClientTemplate**
> ClientTemplateResponse getClientTemplate()


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let templateId: number; // (default to undefined)

const { status, data } = await apiInstance.getClientTemplate(
    templateId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateId** | [**number**] |  | defaults to undefined|


### Return type

**ClientTemplateResponse**

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

# **getClientTemplates**
> ClientTemplateResponseList getClientTemplates()


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let templateType: ClientTemplateType; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getClientTemplates(
    templateType,
    offset,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateType** | **ClientTemplateType** |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|


### Return type

**ClientTemplateResponseList**

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

# **getClientTemplatesSimple**
> ClientTemplatesSimpleResponse getClientTemplatesSimple()


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let templateType: ClientTemplateType; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let all: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getClientTemplatesSimple(
    templateType,
    offset,
    limit,
    search,
    sort,
    all
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateType** | **ClientTemplateType** |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|
| **all** | [**boolean**] |  | (optional) defaults to false|


### Return type

**ClientTemplatesSimpleResponse**

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

# **modifyClientTemplate**
> ClientTemplateResponse modifyClientTemplate(clientTemplateModify)


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration,
    ClientTemplateModify
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let templateId: number; // (default to undefined)
let clientTemplateModify: ClientTemplateModify; //

const { status, data } = await apiInstance.modifyClientTemplate(
    templateId,
    clientTemplateModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **clientTemplateModify** | **ClientTemplateModify**|  | |
| **templateId** | [**number**] |  | defaults to undefined|


### Return type

**ClientTemplateResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeClientTemplate**
> removeClientTemplate()


### Example

```typescript
import {
    ClientTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new ClientTemplateApi(configuration);

let templateId: number; // (default to undefined)

const { status, data } = await apiInstance.removeClientTemplate(
    templateId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateId** | [**number**] |  | defaults to undefined|


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

