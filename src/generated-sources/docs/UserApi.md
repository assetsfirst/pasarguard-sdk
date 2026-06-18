# UserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**activeNextPlan**](#activenextplan) | **POST** /api/user/{username}/active_next | Active Next Plan|
|[**activeNextPlanById**](#activenextplanbyid) | **POST** /api/user/by-id/{user_id}/active_next | Active Next Plan By Id|
|[**activeNextPlanByUsername**](#activenextplanbyusername) | **POST** /api/user/by-username/{username}/active_next | Active Next Plan By Username|
|[**bulkApplyTemplateToUsers**](#bulkapplytemplatetousers) | **POST** /api/users/bulk/apply_template | Bulk Apply Template To Users|
|[**bulkCreateUsersFromTemplate**](#bulkcreateusersfromtemplate) | **POST** /api/users/bulk/from_template | Bulk Create Users From Template|
|[**bulkDeleteUsers**](#bulkdeleteusers) | **POST** /api/users/bulk/delete | Bulk Delete Users|
|[**bulkDisableUsers**](#bulkdisableusers) | **POST** /api/users/bulk/disable | Bulk Disable Users|
|[**bulkEnableUsers**](#bulkenableusers) | **POST** /api/users/bulk/enable | Bulk Enable Users|
|[**bulkModifyUsersDatalimit**](#bulkmodifyusersdatalimit) | **POST** /api/users/bulk/data_limit | Bulk sum/sub to data limit of users|
|[**bulkModifyUsersExpire**](#bulkmodifyusersexpire) | **POST** /api/users/bulk/expire | Bulk sum/sub to expire of users|
|[**bulkModifyUsersProxySettings**](#bulkmodifyusersproxysettings) | **POST** /api/users/bulk/proxy_settings | Bulk modify users proxy settings|
|[**bulkReallocateWireguardPeerIps**](#bulkreallocatewireguardpeerips) | **POST** /api/users/bulk/wireguard/reallocate-peer-ips | Bulk reallocate WireGuard peer IPs|
|[**bulkResetUsersDataUsage**](#bulkresetusersdatausage) | **POST** /api/users/bulk/reset | Bulk Reset Users Data Usage|
|[**bulkRevokeUsersSubscription**](#bulkrevokeuserssubscription) | **POST** /api/users/bulk/revoke_sub | Bulk Revoke Users Subscription|
|[**bulkSetOwner**](#bulksetowner) | **PUT** /api/users/bulk/set_owner | Bulk Set Owner|
|[**createUser**](#createuser) | **POST** /api/user | Create User|
|[**createUserFromTemplate**](#createuserfromtemplate) | **POST** /api/user/from_template | Create User From Template|
|[**deleteExpiredUsers**](#deleteexpiredusers) | **DELETE** /api/users/expired | Delete Expired Users|
|[**getExpiredUsers**](#getexpiredusers) | **GET** /api/users/expired | Get Expired Users|
|[**getUser**](#getuser) | **GET** /api/user/{username} | Get User|
|[**getUserById**](#getuserbyid) | **GET** /api/user/by-id/{user_id} | Get User By Id|
|[**getUserByUsername**](#getuserbyusername) | **GET** /api/user/by-username/{username} | Get User By Username|
|[**getUserSubUpdateList**](#getusersubupdatelist) | **GET** /api/user/{username}/sub_update | Get User Sub Update List|
|[**getUserSubUpdateListById**](#getusersubupdatelistbyid) | **GET** /api/user/by-id/{user_id}/sub_update | Get User Sub Update List By Id|
|[**getUserSubUpdateListByUsername**](#getusersubupdatelistbyusername) | **GET** /api/user/by-username/{username}/sub_update | Get User Sub Update List By Username|
|[**getUserSubscriptionById**](#getusersubscriptionbyid) | **GET** /api/user/{user_id}/subscription/{client_type} | Get User Subscription By Id|
|[**getUserUsage**](#getuserusage) | **GET** /api/user/{username}/usage | Get User Usage|
|[**getUserUsageById**](#getuserusagebyid) | **GET** /api/user/by-id/{user_id}/usage | Get User Usage By Id|
|[**getUserUsageByUsername**](#getuserusagebyusername) | **GET** /api/user/by-username/{username}/usage | Get User Usage By Username|
|[**getUsers**](#getusers) | **GET** /api/users | Get Users|
|[**getUsersCountMetric**](#getuserscountmetric) | **GET** /api/users/counts/{metric} | Get Users Count Metric|
|[**getUsersSimple**](#getuserssimple) | **GET** /api/users/simple | Get lightweight user list|
|[**getUsersSubUpdateChart**](#getuserssubupdatechart) | **GET** /api/users/sub_update/chart | Get Users Sub Update Chart|
|[**getUsersUsage**](#getusersusage) | **GET** /api/users/usage | Get Users Usage|
|[**modifyUser**](#modifyuser) | **PUT** /api/user/{username} | Modify User|
|[**modifyUserById**](#modifyuserbyid) | **PUT** /api/user/by-id/{user_id} | Modify User By Id|
|[**modifyUserByUsername**](#modifyuserbyusername) | **PUT** /api/user/by-username/{username} | Modify User By Username|
|[**modifyUserWithTemplate**](#modifyuserwithtemplate) | **PUT** /api/user/from_template/{username} | Modify User With Template|
|[**modifyUserWithTemplateById**](#modifyuserwithtemplatebyid) | **PUT** /api/user/from_template/by-id/{user_id} | Modify User With Template By Id|
|[**modifyUserWithTemplateByUsername**](#modifyuserwithtemplatebyusername) | **PUT** /api/user/from_template/by-username/{username} | Modify User With Template By Username|
|[**removeUser**](#removeuser) | **DELETE** /api/user/{username} | Remove User|
|[**removeUserById**](#removeuserbyid) | **DELETE** /api/user/by-id/{user_id} | Remove User By Id|
|[**removeUserByUsername**](#removeuserbyusername) | **DELETE** /api/user/by-username/{username} | Remove User By Username|
|[**resetUserDataUsage**](#resetuserdatausage) | **POST** /api/user/{username}/reset | Reset User Data Usage|
|[**resetUserDataUsageById**](#resetuserdatausagebyid) | **POST** /api/user/by-id/{user_id}/reset | Reset User Data Usage By Id|
|[**resetUserDataUsageByUsername**](#resetuserdatausagebyusername) | **POST** /api/user/by-username/{username}/reset | Reset User Data Usage By Username|
|[**resetUsersDataUsage**](#resetusersdatausage) | **POST** /api/users/reset | Reset Users Data Usage|
|[**revokeUserSubscription**](#revokeusersubscription) | **POST** /api/user/{username}/revoke_sub | Revoke User Subscription|
|[**revokeUserSubscriptionById**](#revokeusersubscriptionbyid) | **POST** /api/user/by-id/{user_id}/revoke_sub | Revoke User Subscription By Id|
|[**revokeUserSubscriptionByUsername**](#revokeusersubscriptionbyusername) | **POST** /api/user/by-username/{username}/revoke_sub | Revoke User Subscription By Username|
|[**setOwner**](#setowner) | **PUT** /api/user/{username}/set_owner | Set Owner|
|[**setOwnerById**](#setownerbyid) | **PUT** /api/user/by-id/{user_id}/set_owner | Set Owner By Id|
|[**setOwnerByUsername**](#setownerbyusername) | **PUT** /api/user/by-username/{username}/set_owner | Set Owner By Username|
|[**setUserDisabled**](#setuserdisabled) | **PUT** /api/user/{username}/disabled | Set User Disabled|
|[**setUserDisabledById**](#setuserdisabledbyid) | **PUT** /api/user/by-id/{user_id}/disabled | Set User Disabled By Id|
|[**setUserDisabledByUsername**](#setuserdisabledbyusername) | **PUT** /api/user/by-username/{username}/disabled | Set User Disabled By Username|

# **activeNextPlan**
> UserResponse activeNextPlan()

Reset user by next plan

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.activeNextPlan(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **activeNextPlanById**
> UserResponse activeNextPlanById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.activeNextPlanById(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **activeNextPlanByUsername**
> UserResponse activeNextPlanByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.activeNextPlanByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **bulkApplyTemplateToUsers**
> BulkUsersActionResponse bulkApplyTemplateToUsers(bulkUsersApplyTemplate)

Apply a user template to selected existing users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersApplyTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersApplyTemplate: BulkUsersApplyTemplate; //

const { status, data } = await apiInstance.bulkApplyTemplateToUsers(
    bulkUsersApplyTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersApplyTemplate** | **BulkUsersApplyTemplate**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkCreateUsersFromTemplate**
> BulkUsersCreateResponse bulkCreateUsersFromTemplate(bulkUsersFromTemplate)

Bulk create users from a template using configurable username strategies.  - Includes the template creation fields plus `count`, `strategy`, and `start_number` (for sequences). - **strategy**: Username generation strategy — `sequence` or `random`. - **start_number**: Optional starting suffix for `sequence` strategy. Defaults to `1` and does not parse numbers from the base username.  Returns subscription URLs for created users.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersFromTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersFromTemplate: BulkUsersFromTemplate; //

const { status, data } = await apiInstance.bulkCreateUsersFromTemplate(
    bulkUsersFromTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersFromTemplate** | **BulkUsersFromTemplate**|  | |


### Return type

**BulkUsersCreateResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkDeleteUsers**
> RemoveUsersResponse bulkDeleteUsers(bulkUsersSelection)

Delete selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSelection: BulkUsersSelection; //

const { status, data } = await apiInstance.bulkDeleteUsers(
    bulkUsersSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSelection** | **BulkUsersSelection**|  | |


### Return type

**RemoveUsersResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkDisableUsers**
> BulkUsersActionResponse bulkDisableUsers(bulkUsersSelection)

Disable selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSelection: BulkUsersSelection; //

const { status, data } = await apiInstance.bulkDisableUsers(
    bulkUsersSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSelection** | **BulkUsersSelection**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkEnableUsers**
> BulkUsersActionResponse bulkEnableUsers(bulkUsersSelection)

Enable selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSelection: BulkUsersSelection; //

const { status, data } = await apiInstance.bulkEnableUsers(
    bulkUsersSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSelection** | **BulkUsersSelection**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkModifyUsersDatalimit**
> any bulkModifyUsersDatalimit(bulkUser)

Bulk modify users\' data limit based on the provided criteria.  - **amount**: amount to adjust the user\'s quota (positive to increase, negative to decrease) required - **user_ids**: Optional list of user IDs to modify - **admins**: Optional list of admin IDs — their users will be targeted - **status**: Optional status to filter users (e.g., \"expired\", \"active\"), Empty means no filtering - **group_ids**: Optional list of group IDs to filter users by their group membership - **expire_after**: Optional UTC datetime to filter users whose expire date is on or after this date - **expire_before**: Optional UTC datetime to filter users whose expire date is on or before this date

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUser
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUser: BulkUser; //

const { status, data } = await apiInstance.bulkModifyUsersDatalimit(
    bulkUser
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUser** | **BulkUser**|  | |


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkModifyUsersExpire**
> any bulkModifyUsersExpire(bulkUser)

Bulk expire users based on the provided criteria.  - **amount**: amount to adjust the user\'s quota (in seconds, positive to increase, negative to decrease) required - **user_ids**: Optional list of user IDs to modify - **admins**: Optional list of admin IDs — their users will be targeted - **status**: Optional status to filter users (e.g., \"expired\", \"active\"), Empty means no filtering - **group_ids**: Optional list of group IDs to filter users by their group membership - **expire_after**: Optional UTC datetime to filter users whose expire date is on or after this date - **expire_before**: Optional UTC datetime to filter users whose expire date is on or before this date

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUser
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUser: BulkUser; //

const { status, data } = await apiInstance.bulkModifyUsersExpire(
    bulkUser
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUser** | **BulkUser**|  | |


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkModifyUsersProxySettings**
> any bulkModifyUsersProxySettings(bulkUsersProxy)


### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersProxy
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersProxy: BulkUsersProxy; //

const { status, data } = await apiInstance.bulkModifyUsersProxySettings(
    bulkUsersProxy
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersProxy** | **BulkUsersProxy**|  | |


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkReallocateWireguardPeerIps**
> WireGuardPeerIPsReallocateResponse bulkReallocateWireguardPeerIps(bulkWireGuardPeerIPs)

Same scoping as other bulk user actions (users, admins, group_ids, optional status filter). non-owner admins only affect their own users.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkWireGuardPeerIPs
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkWireGuardPeerIPs: BulkWireGuardPeerIPs; //

const { status, data } = await apiInstance.bulkReallocateWireguardPeerIps(
    bulkWireGuardPeerIPs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkWireGuardPeerIPs** | **BulkWireGuardPeerIPs**|  | |


### Return type

**WireGuardPeerIPsReallocateResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkResetUsersDataUsage**
> BulkUsersActionResponse bulkResetUsersDataUsage(bulkUsersSelection)

Reset usage for selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSelection: BulkUsersSelection; //

const { status, data } = await apiInstance.bulkResetUsersDataUsage(
    bulkUsersSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSelection** | **BulkUsersSelection**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkRevokeUsersSubscription**
> BulkUsersActionResponse bulkRevokeUsersSubscription(bulkUsersSelection)

Revoke subscriptions for selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSelection
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSelection: BulkUsersSelection; //

const { status, data } = await apiInstance.bulkRevokeUsersSubscription(
    bulkUsersSelection
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSelection** | **BulkUsersSelection**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bulkSetOwner**
> BulkUsersActionResponse bulkSetOwner(bulkUsersSetOwner)

Set a new owner for selected users by ID.

### Example

```typescript
import {
    UserApi,
    Configuration,
    BulkUsersSetOwner
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let bulkUsersSetOwner: BulkUsersSetOwner; //

const { status, data } = await apiInstance.bulkSetOwner(
    bulkUsersSetOwner
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bulkUsersSetOwner** | **BulkUsersSetOwner**|  | |


### Return type

**BulkUsersActionResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createUser**
> UserResponse createUser(userCreate)

Create a new user  - **username**: 3 to 32 characters, can include a-z, 0-9, and underscores. - **status**: User\'s status, defaults to `active`. Special rules if `on_hold`. - **expire**: UTC datetime for account expiration. Use `0` for unlimited. - **data_limit**: Max data usage in bytes (e.g., `1073741824` for 1GB). `0` means unlimited. - **data_limit_reset_strategy**: Defines how/if data limit resets. `no_reset` means it never resets. - **proxy_settings**: Dictionary of protocol settings (e.g., `vmess`, `vless`) will generate data for all protocol by default. - **group_ids**: List of group IDs to assign to the user. - **note**: Optional text field for additional user information or notes. - **on_hold_timeout**: UTC timestamp when `on_hold` status should start or end. - **on_hold_expire_duration**: Duration (in seconds) for how long the user should stay in `on_hold` status. - **next_plan**: Next user plan (resets after use).

### Example

```typescript
import {
    UserApi,
    Configuration,
    UserCreate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userCreate: UserCreate; //

const { status, data } = await apiInstance.createUser(
    userCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userCreate** | **UserCreate**|  | |


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**409** | Conflict Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createUserFromTemplate**
> UserResponse createUserFromTemplate(createUserFromTemplate)


### Example

```typescript
import {
    UserApi,
    Configuration,
    CreateUserFromTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let createUserFromTemplate: CreateUserFromTemplate; //

const { status, data } = await apiInstance.createUserFromTemplate(
    createUserFromTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUserFromTemplate** | **CreateUserFromTemplate**|  | |


### Return type

**UserResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteExpiredUsers**
> RemoveUsersResponse deleteExpiredUsers()

Delete cleanup-target users in the specified scope.  - **target**: `expired` (time-based) or `limited` (usage-based) - **expired_after** UTC datetime (optional) - **expired_before** UTC datetime (optional) - Date range filters are applied only when target is `expired`

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let adminUsername: string; // (optional) (default to undefined)
let target: 'expired' | 'limited'; // (optional) (default to 'expired')
let expiredAfter: string; // (optional) (default to undefined)
let expiredBefore: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.deleteExpiredUsers(
    adminUsername,
    target,
    expiredAfter,
    expiredBefore
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminUsername** | [**string**] |  | (optional) defaults to undefined|
| **target** | [**&#39;expired&#39; | &#39;limited&#39;**]**Array<&#39;expired&#39; &#124; &#39;limited&#39;>** |  | (optional) defaults to 'expired'|
| **expiredAfter** | [**string**] |  | (optional) defaults to undefined|
| **expiredBefore** | [**string**] |  | (optional) defaults to undefined|


### Return type

**RemoveUsersResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getExpiredUsers**
> Array<string | null> getExpiredUsers()

Get cleanup-target users in the specified scope.  - **target**: `expired` (time-based) or `limited` (usage-based) - **expired_after** UTC datetime (optional) - **expired_before** UTC datetime (optional) - Date range filters are applied only when target is `expired`

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let adminUsername: string; // (optional) (default to undefined)
let target: 'expired' | 'limited'; // (optional) (default to 'expired')
let expiredAfter: string; // (optional) (default to undefined)
let expiredBefore: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getExpiredUsers(
    adminUsername,
    target,
    expiredAfter,
    expiredBefore
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminUsername** | [**string**] |  | (optional) defaults to undefined|
| **target** | [**&#39;expired&#39; | &#39;limited&#39;**]**Array<&#39;expired&#39; &#124; &#39;limited&#39;>** |  | (optional) defaults to 'expired'|
| **expiredAfter** | [**string**] |  | (optional) defaults to undefined|
| **expiredBefore** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<string | null>**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUser**
> UserResponse getUser()

Get user information

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.getUser(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **getUserById**
> UserResponse getUserById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.getUserById(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **getUserByUsername**
> UserResponse getUserByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.getUserByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **getUserSubUpdateList**
> UserSubscriptionUpdateList getUserSubUpdateList()

Get user subscription agent list

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let offset: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getUserSubUpdateList(
    username,
    offset,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**UserSubscriptionUpdateList**

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

# **getUserSubUpdateListById**
> UserSubscriptionUpdateList getUserSubUpdateListById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let offset: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getUserSubUpdateListById(
    userId,
    offset,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**UserSubscriptionUpdateList**

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

# **getUserSubUpdateListByUsername**
> UserSubscriptionUpdateList getUserSubUpdateListByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let offset: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getUserSubUpdateListByUsername(
    username,
    offset,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**UserSubscriptionUpdateList**

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

# **getUserSubscriptionById**
> any getUserSubscriptionById()

Get a user\'s subscription content in the requested format.

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let clientType: ConfigFormat; // (default to undefined)

const { status, data } = await apiInstance.getUserSubscriptionById(
    userId,
    clientType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|
| **clientType** | **ConfigFormat** |  | defaults to undefined|


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

# **getUserUsage**
> UserUsageStatsList getUserUsage()

Get users usage

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserUsage(
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

# **getUserUsageById**
> UserUsageStatsList getUserUsageById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserUsageById(
    userId,
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
| **userId** | [**number**] |  | defaults to undefined|
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

# **getUserUsageByUsername**
> UserUsageStatsList getUserUsageByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserUsageByUsername(
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

# **getUsers**
> UsersResponse getUsers()

Get all users

### Example

```typescript
import {
    UserApi,
    Configuration,
    Status1
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let ids: Array<number>; // (optional) (default to undefined)
let username: Array<string>; // (optional) (default to undefined)
let usernames: Array<string>; // (optional) (default to undefined)
let admin: Array<string>; // (optional) (default to undefined)
let adminIds: Array<number>; // (optional) (default to undefined)
let group: Array<number>; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let status: Status1; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let proxyId: string; // (optional) (default to undefined)
let dataLimitResetStrategy: Array<DataLimitResetStrategy>; // (optional) (default to undefined)
let dataLimitMin: number; // (optional) (default to undefined)
let dataLimitMax: number; // (optional) (default to undefined)
let expireAfter: string; // (optional) (default to undefined)
let expireBefore: string; // (optional) (default to undefined)
let onlineAfter: string; // (optional) (default to undefined)
let onlineBefore: string; // (optional) (default to undefined)
let online: boolean; // (optional) (default to false)
let noDataLimit: boolean; // (optional) (default to false)
let noExpire: boolean; // (optional) (default to false)
let loadSub: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getUsers(
    offset,
    limit,
    ids,
    username,
    usernames,
    admin,
    adminIds,
    group,
    search,
    status,
    sort,
    proxyId,
    dataLimitResetStrategy,
    dataLimitMin,
    dataLimitMax,
    expireAfter,
    expireBefore,
    onlineAfter,
    onlineBefore,
    online,
    noDataLimit,
    noExpire,
    loadSub
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **ids** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **username** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **usernames** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **admin** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **adminIds** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **group** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **status** | **Status1** |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|
| **proxyId** | [**string**] |  | (optional) defaults to undefined|
| **dataLimitResetStrategy** | **Array&lt;DataLimitResetStrategy&gt;** |  | (optional) defaults to undefined|
| **dataLimitMin** | [**number**] |  | (optional) defaults to undefined|
| **dataLimitMax** | [**number**] |  | (optional) defaults to undefined|
| **expireAfter** | [**string**] |  | (optional) defaults to undefined|
| **expireBefore** | [**string**] |  | (optional) defaults to undefined|
| **onlineAfter** | [**string**] |  | (optional) defaults to undefined|
| **onlineBefore** | [**string**] |  | (optional) defaults to undefined|
| **online** | [**boolean**] |  | (optional) defaults to false|
| **noDataLimit** | [**boolean**] |  | (optional) defaults to false|
| **noExpire** | [**boolean**] |  | (optional) defaults to false|
| **loadSub** | [**boolean**] |  | (optional) defaults to false|


### Return type

**UsersResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUsersCountMetric**
> UserCountMetricStatsList getUsersCountMetric()

Get one users activity/status count metric from usage rows.

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let metric: UserCountMetric; // (default to undefined)
let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)
let admin: Array<string>; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUsersCountMetric(
    metric,
    period,
    nodeId,
    groupByNode,
    start,
    end,
    admin
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **metric** | **UserCountMetric** |  | defaults to undefined|
| **period** | **Period** |  | (optional) defaults to undefined|
| **nodeId** | [**number**] |  | (optional) defaults to undefined|
| **groupByNode** | [**boolean**] |  | (optional) defaults to false|
| **start** | [**string**] |  | (optional) defaults to undefined|
| **end** | [**string**] |  | (optional) defaults to undefined|
| **admin** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|


### Return type

**UserCountMetricStatsList**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUsersSimple**
> UsersSimpleResponse getUsersSimple()

Returns only id and username for users. Optimized for dropdowns and autocomplete.

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let ids: Array<number>; // (optional) (default to undefined)
let usernames: Array<string>; // (optional) (default to undefined)
let offset: number; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let search: string; // (optional) (default to undefined)
let sort: string; // (optional) (default to undefined)
let all: boolean; // (optional) (default to false)

const { status, data } = await apiInstance.getUsersSimple(
    ids,
    usernames,
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
| **ids** | **Array&lt;number&gt;** |  | (optional) defaults to undefined|
| **usernames** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|
| **offset** | [**number**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **search** | [**string**] |  | (optional) defaults to undefined|
| **sort** | [**string**] |  | (optional) defaults to undefined|
| **all** | [**boolean**] |  | (optional) defaults to false|


### Return type

**UsersSimpleResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUsersSubUpdateChart**
> UserSubscriptionUpdateChart getUsersSubUpdateChart()

Get subscription agent distribution percentages (optionally filtered by user_id/username).

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (optional) (default to undefined)
let username: string; // (optional) (default to undefined)
let adminId: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUsersSubUpdateChart(
    userId,
    username,
    adminId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | (optional) defaults to undefined|
| **username** | [**string**] |  | (optional) defaults to undefined|
| **adminId** | [**number**] |  | (optional) defaults to undefined|


### Return type

**UserSubscriptionUpdateChart**

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

# **getUsersUsage**
> UserUsageStatsList getUsersUsage()

Get all users usage

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let period: Period; // (optional) (default to undefined)
let nodeId: number; // (optional) (default to undefined)
let groupByNode: boolean; // (optional) (default to false)
let start: string; // (optional) (default to undefined)
let end: string; // (optional) (default to undefined)
let admin: Array<string>; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUsersUsage(
    period,
    nodeId,
    groupByNode,
    start,
    end,
    admin
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **period** | **Period** |  | (optional) defaults to undefined|
| **nodeId** | [**number**] |  | (optional) defaults to undefined|
| **groupByNode** | [**boolean**] |  | (optional) defaults to false|
| **start** | [**string**] |  | (optional) defaults to undefined|
| **end** | [**string**] |  | (optional) defaults to undefined|
| **admin** | **Array&lt;string&gt;** |  | (optional) defaults to undefined|


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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUser**
> UserResponse modifyUser(userModify)

Modify an existing user  - **username**: Cannot be changed. Used to identify the user. - **status**: User\'s new status. Can be \'active\', \'disabled\', \'on_hold\', \'limited\', or \'expired\'. - **expire**: UTC datetime for new account expiration. Set to `0` for unlimited, `null` for no change. - **data_limit**: New max data usage in bytes (e.g., `1073741824` for 1GB). Set to `0` for unlimited, `null` for no change. - **data_limit_reset_strategy**: New strategy for data limit reset. Options include \'daily\', \'weekly\', \'monthly\', or \'no_reset\'. - **proxies**: Dictionary of new protocol settings (e.g., `vmess`, `vless`). Empty dictionary means no change. - **group_ids**: List of new group IDs to assign to the user. Empty list means no change. - **note**: New optional text for additional user information or notes. `null` means no change. - **on_hold_timeout**: New UTC timestamp for when `on_hold` status should start or end. Only applicable if status is changed to \'on_hold\'. - **on_hold_expire_duration**: New duration (in seconds) for how long the user should stay in `on_hold` status. Only applicable if status is changed to \'on_hold\'. - **next_plan**: Next user plan (resets after use).  Note: Fields set to `null` or omitted will not be modified.

### Example

```typescript
import {
    UserApi,
    Configuration,
    UserModify
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let userModify: UserModify; //

const { status, data } = await apiInstance.modifyUser(
    username,
    userModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userModify** | **UserModify**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserById**
> UserResponse modifyUserById(userModify)


### Example

```typescript
import {
    UserApi,
    Configuration,
    UserModify
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let userModify: UserModify; //

const { status, data } = await apiInstance.modifyUserById(
    userId,
    userModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userModify** | **UserModify**|  | |
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserByUsername**
> UserResponse modifyUserByUsername(userModify)


### Example

```typescript
import {
    UserApi,
    Configuration,
    UserModify
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let userModify: UserModify; //

const { status, data } = await apiInstance.modifyUserByUsername(
    username,
    userModify
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userModify** | **UserModify**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserWithTemplate**
> UserResponse modifyUserWithTemplate(modifyUserByTemplate)


### Example

```typescript
import {
    UserApi,
    Configuration,
    ModifyUserByTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let modifyUserByTemplate: ModifyUserByTemplate; //

const { status, data } = await apiInstance.modifyUserWithTemplate(
    username,
    modifyUserByTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **modifyUserByTemplate** | **ModifyUserByTemplate**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserWithTemplateById**
> UserResponse modifyUserWithTemplateById(modifyUserByTemplate)


### Example

```typescript
import {
    UserApi,
    Configuration,
    ModifyUserByTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let modifyUserByTemplate: ModifyUserByTemplate; //

const { status, data } = await apiInstance.modifyUserWithTemplateById(
    userId,
    modifyUserByTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **modifyUserByTemplate** | **ModifyUserByTemplate**|  | |
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **modifyUserWithTemplateByUsername**
> UserResponse modifyUserWithTemplateByUsername(modifyUserByTemplate)


### Example

```typescript
import {
    UserApi,
    Configuration,
    ModifyUserByTemplate
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let modifyUserByTemplate: ModifyUserByTemplate; //

const { status, data } = await apiInstance.modifyUserWithTemplateByUsername(
    username,
    modifyUserByTemplate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **modifyUserByTemplate** | **ModifyUserByTemplate**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeUser**
> removeUser()

Remove a user

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeUser(
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
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeUserById**
> removeUserById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.removeUserById(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


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

# **removeUserByUsername**
> removeUserByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.removeUserByUsername(
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
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resetUserDataUsage**
> UserResponse resetUserDataUsage()

Reset user data usage

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.resetUserDataUsage(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **resetUserDataUsageById**
> UserResponse resetUserDataUsageById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.resetUserDataUsageById(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **resetUserDataUsageByUsername**
> UserResponse resetUserDataUsageByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.resetUserDataUsageByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **resetUsersDataUsage**
> any resetUsersDataUsage()

Reset all users data usage

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

const { status, data } = await apiInstance.resetUsersDataUsage();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **revokeUserSubscription**
> UserResponse revokeUserSubscription()

Revoke users subscription (Subscription link and proxies)

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.revokeUserSubscription(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **revokeUserSubscriptionById**
> UserResponse revokeUserSubscriptionById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)

const { status, data } = await apiInstance.revokeUserSubscriptionById(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **revokeUserSubscriptionByUsername**
> UserResponse revokeUserSubscriptionByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)

const { status, data } = await apiInstance.revokeUserSubscriptionByUsername(
    username
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **setOwner**
> UserResponse setOwner()

Set a new owner (admin) for a user.

### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let adminUsername: string; // (default to undefined)

const { status, data } = await apiInstance.setOwner(
    username,
    adminUsername
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **adminUsername** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **setOwnerById**
> UserResponse setOwnerById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let adminUsername: string; // (default to undefined)

const { status, data } = await apiInstance.setOwnerById(
    userId,
    adminUsername
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] |  | defaults to undefined|
| **adminUsername** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **setOwnerByUsername**
> UserResponse setOwnerByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let adminUsername: string; // (default to undefined)

const { status, data } = await apiInstance.setOwnerByUsername(
    username,
    adminUsername
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **username** | [**string**] |  | defaults to undefined|
| **adminUsername** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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

# **setUserDisabled**
> UserResponse setUserDisabled(userStatusToggle)


### Example

```typescript
import {
    UserApi,
    Configuration,
    UserStatusToggle
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let userStatusToggle: UserStatusToggle; //

const { status, data } = await apiInstance.setUserDisabled(
    username,
    userStatusToggle
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userStatusToggle** | **UserStatusToggle**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setUserDisabledById**
> UserResponse setUserDisabledById(userStatusToggle)


### Example

```typescript
import {
    UserApi,
    Configuration,
    UserStatusToggle
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userId: number; // (default to undefined)
let userStatusToggle: UserStatusToggle; //

const { status, data } = await apiInstance.setUserDisabledById(
    userId,
    userStatusToggle
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userStatusToggle** | **UserStatusToggle**|  | |
| **userId** | [**number**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setUserDisabledByUsername**
> UserResponse setUserDisabledByUsername(userStatusToggle)


### Example

```typescript
import {
    UserApi,
    Configuration,
    UserStatusToggle
} from './api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let username: string; // (default to undefined)
let userStatusToggle: UserStatusToggle; //

const { status, data } = await apiInstance.setUserDisabledByUsername(
    username,
    userStatusToggle
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userStatusToggle** | **UserStatusToggle**|  | |
| **username** | [**string**] |  | defaults to undefined|


### Return type

**UserResponse**

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
|**400** | BadRequest Error |  -  |
|**403** | Forbidden Error |  -  |
|**404** | NotFound Error |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

