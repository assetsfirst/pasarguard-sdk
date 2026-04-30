# UserTemplateApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bulkDeleteUserTemplates**](#bulkdeleteusertemplates) | **POST** /api/user_templates/bulk/delete | Bulk Delete User Templates|
|[**bulkDisableUserTemplates**](#bulkdisableusertemplates) | **POST** /api/user_templates/bulk/disable | Bulk Disable User Templates|
|[**bulkEnableUserTemplates**](#bulkenableusertemplates) | **POST** /api/user_templates/bulk/enable | Bulk Enable User Templates|
|[**createUserTemplate**](#createusertemplate) | **POST** /api/user_template | Create User Template|
|[**getUserTemplate**](#getusertemplate) | **GET** /api/user_template/{template_id} | Get User Template|
|[**getUserTemplates**](#getusertemplates) | **GET** /api/user_templates | Get User Templates|
|[**getUserTemplatesSimple**](#getusertemplatessimple) | **GET** /api/user_templates/simple | Get lightweight user template list|
|[**modifyUserTemplate**](#modifyusertemplate) | **PUT** /api/user_template/{template_id} | Modify User Template|
|[**removeUserTemplate**](#removeusertemplate) | **DELETE** /api/user_template/{template_id} | Remove User Template|

# **bulkDeleteUserTemplates**
> RemoveUserTemplatesResponse bulkDeleteUserTemplates(bulkUserTemplateSelection)

Delete selected user templates by ID.

### Example

```typescript
import {
    UserTemplateApi,
    Configuration,
    BulkUserTemplateSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let bulkUserTemplateSelection: BulkUserTemplateSelection; //

const { status, data } = await apiInstance.bulkDeleteUserTemplates(
    bulkUserTemplateSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUserTemplateSelection** | **BulkUserTemplateSelection**|  | |


### Return type

**RemoveUserTemplatesResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkDisableUserTemplates**
> BulkUserTemplatesActionResponse bulkDisableUserTemplates(bulkUserTemplateSelection)

Disable selected user templates by ID.

### Example

```typescript
import {
    UserTemplateApi,
    Configuration,
    BulkUserTemplateSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let bulkUserTemplateSelection: BulkUserTemplateSelection; //

const { status, data } = await apiInstance.bulkDisableUserTemplates(
    bulkUserTemplateSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUserTemplateSelection** | **BulkUserTemplateSelection**|  | |


### Return type

**BulkUserTemplatesActionResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkEnableUserTemplates**
> BulkUserTemplatesActionResponse bulkEnableUserTemplates(bulkUserTemplateSelection)

Enable selected user templates by ID.

### Example

```typescript
import {
    UserTemplateApi,
    Configuration,
    BulkUserTemplateSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let bulkUserTemplateSelection: BulkUserTemplateSelection; //

const { status, data } = await apiInstance.bulkEnableUserTemplates(
    bulkUserTemplateSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUserTemplateSelection** | **BulkUserTemplateSelection**|  | |


### Return type

**BulkUserTemplatesActionResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createUserTemplate**
> UserTemplateResponse createUserTemplate(userTemplateCreate)

Create a new user template  - **name** can be up to 64 characters - **data_limit** must be in bytes and larger or equal to 0 - **expire_duration** must be in seconds and larger or equat to 0 - **group_ids** list of group ids

### Example

```typescript
import {
    UserTemplateApi,
    Configuration,
    UserTemplateCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let userTemplateCreate: UserTemplateCreate; //

const { status, data } = await apiInstance.createUserTemplate(
    userTemplateCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userTemplateCreate** | **UserTemplateCreate**|  | |


### Return type

**UserTemplateResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserTemplate**
> UserTemplateResponse getUserTemplate()

Get User Template information with id

### Example

```typescript
import {
    UserTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let templateId: number; // (default to undefined)

const { status, data } = await apiInstance.getUserTemplate(
    templateId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateId** | [**number**] |  | defaults to undefined|


### Return type

**UserTemplateResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserTemplates**
> Array<UserTemplateResponse> getUserTemplates()

Get a list of User Templates with optional pagination

### Example

```typescript
import {
    UserTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserTemplates(
    offset,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|


### Return type

**Array<UserTemplateResponse>**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserTemplatesSimple**
> UserTemplatesSimpleResponse getUserTemplatesSimple()

Returns only id and name for user templates. Optimized for dropdowns and autocomplete.

### Example

```typescript
import {
    UserTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let all: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getUserTemplatesSimple(
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
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|
| **all** | [**boolean**] |  | (optional) defaults to false|


### Return type

**UserTemplatesSimpleResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserTemplate**
> UserTemplateResponse modifyUserTemplate(userTemplateModify)

Modify User Template  - **name** can be up to 64 characters - **data_limit** must be in bytes and larger or equal to 0 - **expire_duration** must be in seconds and larger or equat to 0 - **group_ids** list of group ids

### Example

```typescript
import {
    UserTemplateApi,
    Configuration,
    UserTemplateModify
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let templateId: number; // (default to undefined)
let userTemplateModify: UserTemplateModify; //

const { status, data } = await apiInstance.modifyUserTemplate(
    templateId,
    userTemplateModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userTemplateModify** | **UserTemplateModify**|  | |
| **templateId** | [**number**] |  | defaults to undefined|


### Return type

**UserTemplateResponse**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeUserTemplate**
> removeUserTemplate()

Remove a User Template by its ID

### Example

```typescript
import {
    UserTemplateApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserTemplateApi(configuration);

let templateId: number; // (default to undefined)

const { status, data } = await apiInstance.removeUserTemplate(
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
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

