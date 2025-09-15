# AuthorsApi

All URIs are relative to *http://localhost:8080/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**create**](#create) | **POST** /authors/ | Create author|
|[**deleteById**](#deletebyid) | **DELETE** /authors/{id} | Delete author|
|[**getAll**](#getall) | **GET** /authors/ | List all authors|
|[**getById**](#getbyid) | **GET** /authors/{id} | Get author by ID|
|[**updateById**](#updatebyid) | **PUT** /authors/{id} | Update author|

# **create**
> AuthorsAuthor create(data)

Create a new author

### Example

```typescript
import {
    AuthorsApi,
    Configuration,
    AuthorsCreateAuthorDto
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

let data: AuthorsCreateAuthorDto; //Author data

const { status, data } = await apiInstance.create(
    data
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **data** | **AuthorsCreateAuthorDto**| Author data | |


### Return type

**AuthorsAuthor**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteById**
> deleteById()

Delete an existing author by ID

### Example

```typescript
import {
    AuthorsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

let id: string; //Author ID (default to undefined)

const { status, data } = await apiInstance.deleteById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Author ID | defaults to undefined|


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
|**204** | No Content |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAll**
> Array<AuthorsAuthor> getAll()

Get a list of all authors

### Example

```typescript
import {
    AuthorsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

const { status, data } = await apiInstance.getAll();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<AuthorsAuthor>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getById**
> AuthorsAuthor getById()

Retrieve a single author by their ID

### Example

```typescript
import {
    AuthorsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

let id: string; //Author ID (default to undefined)

const { status, data } = await apiInstance.getById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Author ID | defaults to undefined|


### Return type

**AuthorsAuthor**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**404** | Not Found |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateById**
> AuthorsAuthor updateById(data)

Update an existing author by ID

### Example

```typescript
import {
    AuthorsApi,
    Configuration,
    AuthorsUpdateAuthorDto
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

let id: string; //Author ID (default to undefined)
let data: AuthorsUpdateAuthorDto; //Author data

const { status, data } = await apiInstance.updateById(
    id,
    data
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **data** | **AuthorsUpdateAuthorDto**| Author data | |
| **id** | [**string**] | Author ID | defaults to undefined|


### Return type

**AuthorsAuthor**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |
|**400** | Bad Request |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

