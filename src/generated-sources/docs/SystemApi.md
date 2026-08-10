# SystemApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getInboundDetails**](#getinbounddetails) | **GET** /api/inbounds/details | Get Inbound Details|
|[**getInbounds**](#getinbounds) | **GET** /api/inbounds | Get Inbounds|
|[**getSystemResourceStats**](#getsystemresourcestats) | **GET** /api/system/resources | Get System Resource Stats|
|[**getSystemStats**](#getsystemstats) | **GET** /api/system | Get System Stats|
|[**getSystemUsersStats**](#getsystemusersstats) | **GET** /api/system/users | Get System Users Stats|
|[**getWireguardSubnets**](#getwireguardsubnets) | **GET** /api/wireguard/subnets | Get Wireguard Subnets|
|[**getWorkersHealth**](#getworkershealth) | **GET** /api/workers/health | Get Workers Health|

# **getInboundDetails**
> Array<InboundSummary> getInboundDetails()

Retrieve lightweight inbound metadata for dashboard forms.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.getInboundDetails();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<InboundSummary>**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getInbounds**
> Array<string | null> getInbounds()

Retrieve inbound configurations grouped by protocol.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.getInbounds();
```

### Parameters
This endpoint does not have any parameters.


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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSystemResourceStats**
> SystemResourceStats getSystemResourceStats()

Fetch system resource stats without user metrics.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.getSystemResourceStats();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**SystemResourceStats**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSystemStats**
> SystemStats getSystemStats()

Fetch system stats including memory, CPU, disk, and user metrics.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

let adminUsername: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSystemStats(
    adminUsername
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminUsername** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SystemStats**

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

# **getSystemUsersStats**
> SystemUsersStats getSystemUsersStats()

Fetch user stats and traffic metrics without system resource stats.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

let adminUsername: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSystemUsersStats(
    adminUsername
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adminUsername** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SystemUsersStats**

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

# **getWireguardSubnets**
> Array<WireGuardSubnetUsage> getWireguardSubnets()

Per-subnet WireGuard address usage: capacity, used/free counts and the first free IPs.

### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.getWireguardSubnets();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<WireGuardSubnetUsage>**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getWorkersHealth**
> WorkersHealth getWorkersHealth()


### Example

```typescript
import {
    SystemApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SystemApi(configuration);

const { status, data } = await apiInstance.getWorkersHealth();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**WorkersHealth**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

