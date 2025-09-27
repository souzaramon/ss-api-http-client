# TitlesApi

All URIs are relative to *http://localhost:8080/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTitle**](#createtitle) | **POST** /titles/ | Create title|
|[**deleteTitleById**](#deletetitlebyid) | **DELETE** /titles/{id} | Delete title|
|[**getAllTitles**](#getalltitles) | **GET** /titles/ | List all titles|
|[**getTitleById**](#gettitlebyid) | **GET** /titles/{id} | Get title by ID|
|[**updateTitleById**](#updatetitlebyid) | **PUT** /titles/{id} | Update title|

# **createTitle**
> TitlesTitle createTitle(data)

Create a new title

### Example

```typescript
import {
    TitlesApi,
    Configuration,
    TitlesCreateTitleDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TitlesApi(configuration);

let data: TitlesCreateTitleDto; //Title data

const { status, data } = await apiInstance.createTitle(
    data
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **data** | **TitlesCreateTitleDto**| Title data | |


### Return type

**TitlesTitle**

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

# **deleteTitleById**
> deleteTitleById()

Delete an existing title by ID

### Example

```typescript
import {
    TitlesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TitlesApi(configuration);

let id: string; //Title ID (default to undefined)

const { status, data } = await apiInstance.deleteTitleById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Title ID | defaults to undefined|


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

# **getAllTitles**
> Array<TitlesTitle> getAllTitles()

Get a list of all titles

### Example

```typescript
import {
    TitlesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TitlesApi(configuration);

const { status, data } = await apiInstance.getAllTitles();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<TitlesTitle>**

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

# **getTitleById**
> TitlesTitle getTitleById()

Retrieve a single title by their ID

### Example

```typescript
import {
    TitlesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TitlesApi(configuration);

let id: string; //Title ID (default to undefined)

const { status, data } = await apiInstance.getTitleById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Title ID | defaults to undefined|


### Return type

**TitlesTitle**

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

# **updateTitleById**
> TitlesTitle updateTitleById(data)

Update an existing title by ID

### Example

```typescript
import {
    TitlesApi,
    Configuration,
    TitlesUpdateTitleDto
} from './api';

const configuration = new Configuration();
const apiInstance = new TitlesApi(configuration);

let id: string; //Title ID (default to undefined)
let data: TitlesUpdateTitleDto; //Title data

const { status, data } = await apiInstance.updateTitleById(
    id,
    data
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **data** | **TitlesUpdateTitleDto**| Title data | |
| **id** | [**string**] | Title ID | defaults to undefined|


### Return type

**TitlesTitle**

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

