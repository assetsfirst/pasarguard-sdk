# GroupsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bulkAddGroupsToUsers**](#bulkaddgroupstousers) | **POST** /api/groups/bulk/add | Bulk add groups to users|
|[**bulkDeleteGroups**](#bulkdeletegroups) | **POST** /api/groups/bulk/delete | Bulk Delete Groups|
|[**bulkDisableGroups**](#bulkdisablegroups) | **POST** /api/groups/bulk/disable | Bulk Disable Groups|
|[**bulkEnableGroups**](#bulkenablegroups) | **POST** /api/groups/bulk/enable | Bulk Enable Groups|
|[**bulkRemoveUsersFromGroups**](#bulkremoveusersfromgroups) | **POST** /api/groups/bulk/remove | Bulk remove groups from users|
|[**createGroup**](#creategroup) | **POST** /api/group | Create a new group|
|[**getAllGroups**](#getallgroups) | **GET** /api/groups | List all groups|
|[**getGroup**](#getgroup) | **GET** /api/group/{group_id} | Get group details|
|[**getGroupsSimple**](#getgroupssimple) | **GET** /api/groups/simple | Get lightweight group list|
|[**modifyGroup**](#modifygroup) | **PUT** /api/group/{group_id} | Modify group|
|[**removeGroup**](#removegroup) | **DELETE** /api/group/{group_id} | Remove group|

# **bulkAddGroupsToUsers**
> any bulkAddGroupsToUsers(bulkGroup)

Bulk assign groups to multiple users, users under specific admins, or all users.  - **group_ids**: List of group IDs to add (required) - **users**: Optional list of user IDs to assign the groups to - **admins**: Optional list of admin IDs — their users will be targeted  Notes: - If neither \'users\' nor \'admins\' are provided, groups will be added to *all users* - Existing user-group associations will be ignored (no duplication) - Returns list of affected users (those who received new group associations)

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    BulkGroup
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let bulkGroup: BulkGroup; //

const { status, data } = await apiInstance.bulkAddGroupsToUsers(
    bulkGroup
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkGroup** | **BulkGroup**|  | |


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success confirmation |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkDeleteGroups**
> RemoveGroupsResponse bulkDeleteGroups(bulkGroupSelection)

Delete selected groups by ID.

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    BulkGroupSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let bulkGroupSelection: BulkGroupSelection; //

const { status, data } = await apiInstance.bulkDeleteGroups(
    bulkGroupSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkGroupSelection** | **BulkGroupSelection**|  | |


### Return type

**RemoveGroupsResponse**

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

# **bulkDisableGroups**
> BulkGroupsActionResponse bulkDisableGroups(bulkGroupSelection)

Disable selected groups by ID.

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    BulkGroupSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let bulkGroupSelection: BulkGroupSelection; //

const { status, data } = await apiInstance.bulkDisableGroups(
    bulkGroupSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkGroupSelection** | **BulkGroupSelection**|  | |


### Return type

**BulkGroupsActionResponse**

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

# **bulkEnableGroups**
> BulkGroupsActionResponse bulkEnableGroups(bulkGroupSelection)

Enable selected groups by ID.

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    BulkGroupSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let bulkGroupSelection: BulkGroupSelection; //

const { status, data } = await apiInstance.bulkEnableGroups(
    bulkGroupSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkGroupSelection** | **BulkGroupSelection**|  | |


### Return type

**BulkGroupsActionResponse**

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

# **bulkRemoveUsersFromGroups**
> any bulkRemoveUsersFromGroups(bulkGroup)

Bulk remove groups from multiple users, users under specific admins, or all users.  - **group_ids**: List of group IDs to remove (required) - **users**: Optional list of user IDs to remove the groups from - **admins**: Optional list of admin IDs — their users will be targeted  Notes: - If neither \'users\' nor \'admins\' are provided, groups will be removed from *all users* - Only existing user-group associations will be removed - Returns list of affected users (those who had groups removed)

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    BulkGroup
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let bulkGroup: BulkGroup; //

const { status, data } = await apiInstance.bulkRemoveUsersFromGroups(
    bulkGroup
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkGroup** | **BulkGroup**|  | |


### Return type

**any**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success confirmation |  -  |
|**401** | Unauthorized Error |  * WWW-Authenticate - Authentication type <br>  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createGroup**
> GroupResponse createGroup(groupCreate)

Creates a new group in the system. Only sudo administrators can create groups.

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    GroupCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let groupCreate: GroupCreate; //

const { status, data } = await apiInstance.createGroup(
    groupCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupCreate** | **GroupCreate**|  | |


### Return type

**GroupResponse**

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

# **getAllGroups**
> GroupsResponse getAllGroups()

Retrieves a paginated list of all groups in the system. Requires admin authentication.

### Example

```typescript
import {
    GroupsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAllGroups(
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

**GroupsResponse**

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

# **getGroup**
> GroupResponse getGroup()

Retrieves detailed information about a specific group by its ID.

### Example

```typescript
import {
    GroupsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let groupId: number; // (default to undefined)

const { status, data } = await apiInstance.getGroup(
    groupId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupId** | [**number**] |  | defaults to undefined|


### Return type

**GroupResponse**

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

# **getGroupsSimple**
> GroupsSimpleResponse getGroupsSimple()

Returns only id and name for groups. Optimized for dropdowns and autocomplete.

### Example

```typescript
import {
    GroupsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let all: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getGroupsSimple(
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

**GroupsSimpleResponse**

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

# **modifyGroup**
> GroupResponse modifyGroup(groupModify)

Updates an existing group\'s information. Only sudo administrators can modify groups.

### Example

```typescript
import {
    GroupsApi,
    Configuration,
    GroupModify
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let groupId: number; // (default to undefined)
let groupModify: GroupModify; //

const { status, data } = await apiInstance.modifyGroup(
    groupId,
    groupModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupModify** | **GroupModify**|  | |
| **groupId** | [**number**] |  | defaults to undefined|


### Return type

**GroupResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeGroup**
> removeGroup()

Deletes a group from the system. Only sudo administrators can delete groups.

### Example

```typescript
import {
    GroupsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GroupsApi(configuration);

let groupId: number; // (default to undefined)

const { status, data } = await apiInstance.removeGroup(
    groupId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **groupId** | [**number**] |  | defaults to undefined|


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

