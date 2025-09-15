# AuthorsApi

All URIs are relative to *http://localhost:8080/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**authorsGet**](#authorsget) | **GET** /authors/ | List all authors|
|[**authorsIdDelete**](#authorsiddelete) | **DELETE** /authors/{id} | Delete author|
|[**authorsIdGet**](#authorsidget) | **GET** /authors/{id} | Get author by ID|
|[**authorsIdPut**](#authorsidput) | **PUT** /authors/{id} | Update author|
|[**authorsPost**](#authorspost) | **POST** /authors/ | Create author|

# **authorsGet**
> Array<AuthorsAuthor> authorsGet()

Get a list of all authors

### Example

```typescript
import {
    AuthorsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthorsApi(configuration);

const { status, data } = await apiInstance.authorsGet();
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

# **authorsIdDelete**
> authorsIdDelete()

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

const { status, data } = await apiInstance.authorsIdDelete(
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

# **authorsIdGet**
> AuthorsAuthor authorsIdGet()

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

const { status, data } = await apiInstance.authorsIdGet(
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

# **authorsIdPut**
> AuthorsAuthor authorsIdPut(data)

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

const { status, data } = await apiInstance.authorsIdPut(
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

# **authorsPost**
> AuthorsAuthor authorsPost(data)

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

const { status, data } = await apiInstance.authorsPost(
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

