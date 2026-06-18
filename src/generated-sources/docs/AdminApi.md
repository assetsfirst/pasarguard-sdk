# AdminApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**activateAllDisabledUsers**](#activatealldisabledusers) | **POST** /api/admin/{username}/users/activate | Activate All Disabled Users|
|[**activateAllDisabledUsersById**](#activatealldisabledusersbyid) | **POST** /api/admin/by-id/{admin_id}/users/activate | Activate All Disabled Users By Id|
|[**activateAllDisabledUsersByUsername**](#activatealldisabledusersbyusername) | **POST** /api/admin/by-username/{username}/users/activate | Activate All Disabled Users By Username|
|[**adminMiniAppToken**](#adminminiapptoken) | **POST** /api/admin/miniapp/token | Admin Mini App Token|
|[**adminToken**](#admintoken) | **POST** /api/admin/token | Admin Token|
|[**bulkActivateAllDisabledUsers**](#bulkactivatealldisabledusers) | **POST** /api/admins/bulk/users/activate | Bulk Activate All Disabled Users|
|[**bulkDeleteAdmins**](#bulkdeleteadmins) | **POST** /api/admins/bulk/delete | Bulk Delete Admins|
|[**bulkDisableAdmins**](#bulkdisableadmins) | **POST** /api/admins/bulk/disable | Bulk Disable Admins|
|[**bulkDisableAllActiveUsers**](#bulkdisableallactiveusers) | **POST** /api/admins/bulk/users/disable | Bulk Disable All Active Users|
|[**bulkEnableAdmins**](#bulkenableadmins) | **POST** /api/admins/bulk/enable | Bulk Enable Admins|
|[**bulkRemoveAllUsers**](#bulkremoveallusers) | **DELETE** /api/admins/bulk/users | Bulk Remove All Users|
|[**bulkResetAdminsUsage**](#bulkresetadminsusage) | **POST** /api/admins/bulk/reset | Bulk Reset Admins Usage|
|[**createAdmin**](#createadmin) | **POST** /api/admin | Create Admin|
|[**disableAllActiveUsers**](#disableallactiveusers) | **POST** /api/admin/{username}/users/disable | Disable All Active Users|
|[**disableAllActiveUsersById**](#disableallactiveusersbyid) | **POST** /api/admin/by-id/{admin_id}/users/disable | Disable All Active Users By Id|
|[**disableAllActiveUsersByUsername**](#disableallactiveusersbyusername) | **POST** /api/admin/by-username/{username}/users/disable | Disable All Active Users By Username|
|[**getAdminUsage**](#getadminusage) | **GET** /api/admin/{username}/usage | Get Admin Usage|
|[**getAdminUsageById**](#getadminusagebyid) | **GET** /api/admin/by-id/{admin_id}/usage | Get Admin Usage By Id|
|[**getAdminUsageByUsername**](#getadminusagebyusername) | **GET** /api/admin/by-username/{username}/usage | Get Admin Usage By Username|
|[**getAdmins**](#getadmins) | **GET** /api/admins | Get Admins|
|[**getAdminsSimple**](#getadminssimple) | **GET** /api/admins/simple | Get lightweight admin list|
|[**getCurrentAdmin**](#getcurrentadmin) | **GET** /api/admin | Get Current Admin|
|[**modifyAdmin**](#modifyadmin) | **PUT** /api/admin/{username} | Modify Admin|
|[**modifyAdminById**](#modifyadminbyid) | **PUT** /api/admin/by-id/{admin_id} | Modify Admin By Id|
|[**modifyAdminByUsername**](#modifyadminbyusername) | **PUT** /api/admin/by-username/{username} | Modify Admin By Username|
|[**removeAdmin**](#removeadmin) | **DELETE** /api/admin/{username} | Remove Admin|
|[**removeAdminById**](#removeadminbyid) | **DELETE** /api/admin/by-id/{admin_id} | Remove Admin By Id|
|[**removeAdminByUsername**](#removeadminbyusername) | **DELETE** /api/admin/by-username/{username} | Remove Admin By Username|
|[**removeAllUsers**](#removeallusers) | **DELETE** /api/admin/{username}/users | Remove All Users|
|[**removeAllUsersById**](#removeallusersbyid) | **DELETE** /api/admin/by-id/{admin_id}/users | Remove All Users By Id|
|[**removeAllUsersByUsername**](#removeallusersbyusername) | **DELETE** /api/admin/by-username/{username}/users | Remove All Users By Username|
|[**resetAdminUsage**](#resetadminusage) | **POST** /api/admin/{username}/reset | Reset Admin Usage|
|[**resetAdminUsageById**](#resetadminusagebyid) | **POST** /api/admin/by-id/{admin_id}/reset | Reset Admin Usage By Id|
|[**resetAdminUsageByUsername**](#resetadminusagebyusername) | **POST** /api/admin/by-username/{username}/reset | Reset Admin Usage By Username|

# **activateAllDisabledUsers**
> any activateAllDisabledUsers()

Activate all disabled users under a specific admin.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.activateAllDisabledUsers(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **activateAllDisabledUsersById**
> any activateAllDisabledUsersById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)

const { status, data } = await apiInstance.activateAllDisabledUsersById(
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|


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

# **activateAllDisabledUsersByUsername**
> any activateAllDisabledUsersByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.activateAllDisabledUsersByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **adminMiniAppToken**
> any adminMiniAppToken()

Authenticate an admin via Telegram MiniApp and issue a token.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let xTelegramAuthorization: string; // (default to undefined)

const { status, data } = await apiInstance.adminMiniAppToken(
    xTelegramAuthorization
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **xTelegramAuthorization** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **adminToken**
> Token adminToken()

Authenticate an admin and issue a token.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)
let password: string; // (default to undefined)
let grantType: string; // (optional) (default to undefined)
let scope: string; // (optional) (default to '')
let clientId: string; // (optional) (default to undefined)
let clientSecret: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.adminToken(
    username,
    password,
    grantType,
    scope,
    clientId,
    clientSecret
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **password** | [**string**] |  | defaults to undefined|
| **grantType** | [**string**] |  | (optional) defaults to undefined|
| **scope** | [**string**] |  | (optional) defaults to ''|
| **clientId** | [**string**] |  | (optional) defaults to undefined|
| **clientSecret** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Token**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkActivateAllDisabledUsers**
> BulkAdminsActionResponse bulkActivateAllDisabledUsers(bulkAdminSelection)

Activate all disabled users under selected admins.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkActivateAllDisabledUsers(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **bulkDeleteAdmins**
> RemoveAdminsResponse bulkDeleteAdmins(bulkAdminSelection)

Delete selected admins by ID.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkDeleteAdmins(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**RemoveAdminsResponse**

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

# **bulkDisableAdmins**
> BulkAdminsActionResponse bulkDisableAdmins(bulkAdminSelection)

Disable selected admins by ID.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkDisableAdmins(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **bulkDisableAllActiveUsers**
> BulkAdminsActionResponse bulkDisableAllActiveUsers(bulkAdminSelection)

Disable all active users under selected admins.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkDisableAllActiveUsers(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **bulkEnableAdmins**
> BulkAdminsActionResponse bulkEnableAdmins(bulkAdminSelection)

Enable selected admins by ID.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkEnableAdmins(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **bulkRemoveAllUsers**
> BulkAdminsActionResponse bulkRemoveAllUsers(bulkAdminSelection)

Remove all users under selected admins.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkRemoveAllUsers(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **bulkResetAdminsUsage**
> BulkAdminsActionResponse bulkResetAdminsUsage(bulkAdminSelection)

Reset usage for selected admins by ID.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    BulkAdminSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let bulkAdminSelection: BulkAdminSelection; //

const { status, data } = await apiInstance.bulkResetAdminsUsage(
    bulkAdminSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkAdminSelection** | **BulkAdminSelection**|  | |


### Return type

**BulkAdminsActionResponse**

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

# **createAdmin**
> AdminDetails createAdmin(adminCreate)

Create a new admin.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    AdminCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminCreate: AdminCreate; //

const { status, data } = await apiInstance.createAdmin(
    adminCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminCreate** | **AdminCreate**|  | |


### Return type

**AdminDetails**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Admin created successfully |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **disableAllActiveUsers**
> any disableAllActiveUsers()

Disable all active users under a specific admin.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.disableAllActiveUsers(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **disableAllActiveUsersById**
> any disableAllActiveUsersById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)

const { status, data } = await apiInstance.disableAllActiveUsersById(
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|


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

# **disableAllActiveUsersByUsername**
> any disableAllActiveUsersByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.disableAllActiveUsersByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **getAdminUsage**
> UserUsageStatsList getAdminUsage()

Get admin usage aggregated from user traffic.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAdminUsage(
    username,
    period,
    nodeId,
    groupByNode,
    start,
    end
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **period** | **Period** |  | (optional) defaults to undefined|
| **nodeId** | [**number**] |  | (optional) defaults to undefined|
| **groupByNode** | [**boolean**] |  | (optional) defaults to false|
| **start** | [**string**] |  | (optional) defaults to undefined|
| **end** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserUsageStatsList**

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

# **getAdminUsageById**
> UserUsageStatsList getAdminUsageById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAdminUsageById(
    adminId,
    period,
    nodeId,
    groupByNode,
    start,
    end
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|
| **period** | **Period** |  | (optional) defaults to undefined|
| **nodeId** | [**number**] |  | (optional) defaults to undefined|
| **groupByNode** | [**boolean**] |  | (optional) defaults to false|
| **start** | [**string**] |  | (optional) defaults to undefined|
| **end** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserUsageStatsList**

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

# **getAdminUsageByUsername**
> UserUsageStatsList getAdminUsageByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAdminUsageByUsername(
    username,
    period,
    nodeId,
    groupByNode,
    start,
    end
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **period** | **Period** |  | (optional) defaults to undefined|
| **nodeId** | [**number**] |  | (optional) defaults to undefined|
| **groupByNode** | [**boolean**] |  | (optional) defaults to false|
| **start** | [**string**] |  | (optional) defaults to undefined|
| **end** | [**string**] |  | (optional) defaults to undefined|


### Return type

**UserUsageStatsList**

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

# **getAdmins**
> AdminsResponse getAdmins()

Fetch a list of admins with optional filters for pagination and username.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let ids: Array<number>; // (optional) (default to undefined)
let usernames: Array<string>; // (optional) (default to undefined)
let username: string; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAdmins(
    ids,
    usernames,
    username,
    offset,
    limit,
    sort
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ids** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **usernames** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **username** | [**string**] |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AdminsResponse**

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

# **getAdminsSimple**
> AdminsSimpleResponse getAdminsSimple()

Returns only id and username for admins. Optimized for dropdowns and autocomplete.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let ids: Array<number>; // (optional) (default to undefined)
let usernames: Array<string>; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let all: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getAdminsSimple(
    ids,
    usernames,
    search,
    offset,
    limit,
    sort,
    all
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ids** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **usernames** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|
| **all** | [**boolean**] |  | (optional) defaults to false|


### Return type

**AdminsSimpleResponse**

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

# **getCurrentAdmin**
> AdminDetails getCurrentAdmin()

Retrieve the current authenticated admin.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

const { status, data } = await apiInstance.getCurrentAdmin();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**AdminDetails**

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

# **modifyAdmin**
> AdminDetails modifyAdmin(adminModify)

Modify an existing admin\'s details.

### Example

```typescript
import {
    AdminApi,
    Configuration,
    AdminModify
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)
let adminModify: AdminModify; //

const { status, data } = await apiInstance.modifyAdmin(
    username,
    adminModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminModify** | **AdminModify**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

# **modifyAdminById**
> AdminDetails modifyAdminById(adminModify)


### Example

```typescript
import {
    AdminApi,
    Configuration,
    AdminModify
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)
let adminModify: AdminModify; //

const { status, data } = await apiInstance.modifyAdminById(
    adminId,
    adminModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminModify** | **AdminModify**|  | |
| **adminId** | [**number**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

# **modifyAdminByUsername**
> AdminDetails modifyAdminByUsername(adminModify)


### Example

```typescript
import {
    AdminApi,
    Configuration,
    AdminModify
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)
let adminModify: AdminModify; //

const { status, data } = await apiInstance.modifyAdminByUsername(
    username,
    adminModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminModify** | **AdminModify**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

# **removeAdmin**
> removeAdmin()

Remove an admin from the database.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeAdmin(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **removeAdminById**
> removeAdminById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)

const { status, data } = await apiInstance.removeAdminById(
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|


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

# **removeAdminByUsername**
> removeAdminByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeAdminByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **removeAllUsers**
> any removeAllUsers()

Remove all users under a specific admin.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeAllUsers(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **removeAllUsersById**
> any removeAllUsersById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)

const { status, data } = await apiInstance.removeAllUsersById(
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|


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

# **removeAllUsersByUsername**
> any removeAllUsersByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeAllUsersByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


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

# **resetAdminUsage**
> AdminDetails resetAdminUsage()

Resets usage of admin.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.resetAdminUsage(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

# **resetAdminUsageById**
> AdminDetails resetAdminUsageById()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let adminId: number; // (default to undefined)

const { status, data } = await apiInstance.resetAdminUsageById(
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminId** | [**number**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

# **resetAdminUsageByUsername**
> AdminDetails resetAdminUsageByUsername()


### Example

```typescript
import {
    AdminApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.resetAdminUsageByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**AdminDetails**

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

