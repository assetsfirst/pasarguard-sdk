# AdminRolesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createRole**](#createrole) | **POST** /api/admin-role | Create Role|
|[**deleteRole**](#deleterole) | **DELETE** /api/admin-role/{role_id} | Delete Role|
|[**getRole**](#getrole) | **GET** /api/admin-role/{role_id} | Get Role|
|[**getRoles**](#getroles) | **GET** /api/admin-roles | Get Roles|
|[**getRolesSimple**](#getrolessimple) | **GET** /api/admin-roles/simple | Get Roles Simple|
|[**modifyRole**](#modifyrole) | **PUT** /api/admin-role/{role_id} | Modify Role|

# **createRole**
> AdminRoleResponse createRole(adminRoleCreate)

Create a new role. Owner only.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration,
    AdminRoleCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

let adminRoleCreate: AdminRoleCreate; //

const { status, data } = await apiInstance.createRole(
    adminRoleCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminRoleCreate** | **AdminRoleCreate**|  | |


### Return type

**AdminRoleResponse**

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

# **deleteRole**
> deleteRole()

Delete a role. Owner only. Built-in roles and in-use roles cannot be deleted.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

let roleId: number; // (default to undefined)

const { status, data } = await apiInstance.deleteRole(
    roleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **roleId** | [**number**] |  | defaults to undefined|


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
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getRole**
> AdminRoleResponse getRole()

Get a role by ID.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

let roleId: number; // (default to undefined)

const { status, data } = await apiInstance.getRole(
    roleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **roleId** | [**number**] |  | defaults to undefined|


### Return type

**AdminRoleResponse**

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

# **getRoles**
> AdminRolesResponse getRoles()

List all roles.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

let search: string; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getRoles(
    search,
    offset,
    limit,
    sort
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AdminRolesResponse**

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

# **getRolesSimple**
> AdminRolesSimpleResponse getRolesSimple()

List all roles as lightweight id/name/is_owner tuples.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

const { status, data } = await apiInstance.getRolesSimple();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**AdminRolesSimpleResponse**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyRole**
> AdminRoleResponse modifyRole(adminRoleModify)

Modify a role. Owner only. Owner role cannot be modified.

### Example

```typescript
import {
    AdminRolesApi,
    Configuration,
    AdminRoleModify
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRolesApi(configuration);

let roleId: number; // (default to undefined)
let adminRoleModify: AdminRoleModify; //

const { status, data } = await apiInstance.modifyRole(
    roleId,
    adminRoleModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminRoleModify** | **AdminRoleModify**|  | |
| **roleId** | [**number**] |  | defaults to undefined|


### Return type

**AdminRoleResponse**

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

