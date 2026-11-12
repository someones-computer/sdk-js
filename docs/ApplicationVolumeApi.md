# ApplicationVolumeApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiApplicationVolumesGetCollection**](ApplicationVolumeApi.md#apiapplicationvolumesgetcollection) | **GET** /api/application_volumes | Retrieves the collection of ApplicationVolume resources. |
| [**apiApplicationVolumesIdDelete**](ApplicationVolumeApi.md#apiapplicationvolumesiddelete) | **DELETE** /api/application_volumes/{id} | Removes the ApplicationVolume resource. |
| [**apiApplicationVolumesIdGet**](ApplicationVolumeApi.md#apiapplicationvolumesidget) | **GET** /api/application_volumes/{id} | Retrieves a ApplicationVolume resource. |



## apiApplicationVolumesGetCollection

> Array&lt;ApplicationVolume&gt; apiApplicationVolumesGetCollection(page)

Retrieves the collection of ApplicationVolume resources.

Retrieves the collection of ApplicationVolume resources.

### Example

```ts
import {
  Configuration,
  ApplicationVolumeApi,
} from '@someones-computer/sdk-js';
import type { ApiApplicationVolumesGetCollectionRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationVolumeApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies ApiApplicationVolumesGetCollectionRequest;

  try {
    const data = await api.apiApplicationVolumesGetCollection(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **page** | `number` | The collection page number | [Optional] [Defaults to `1`] |

### Return type

[**Array&lt;ApplicationVolume&gt;**](ApplicationVolume.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ApplicationVolume collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiApplicationVolumesIdDelete

> apiApplicationVolumesIdDelete(id)

Removes the ApplicationVolume resource.

Removes the ApplicationVolume resource.

### Example

```ts
import {
  Configuration,
  ApplicationVolumeApi,
} from '@someones-computer/sdk-js';
import type { ApiApplicationVolumesIdDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationVolumeApi(config);

  const body = {
    // string | ApplicationVolume identifier
    id: id_example,
  } satisfies ApiApplicationVolumesIdDeleteRequest;

  try {
    const data = await api.apiApplicationVolumesIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` | ApplicationVolume identifier | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/problem+json`, `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | ApplicationVolume resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiApplicationVolumesIdGet

> ApplicationVolume apiApplicationVolumesIdGet(id)

Retrieves a ApplicationVolume resource.

Retrieves a ApplicationVolume resource.

### Example

```ts
import {
  Configuration,
  ApplicationVolumeApi,
} from '@someones-computer/sdk-js';
import type { ApiApplicationVolumesIdGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationVolumeApi(config);

  const body = {
    // string | ApplicationVolume identifier
    id: id_example,
  } satisfies ApiApplicationVolumesIdGetRequest;

  try {
    const data = await api.apiApplicationVolumesIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` | ApplicationVolume identifier | [Defaults to `undefined`] |

### Return type

[**ApplicationVolume**](ApplicationVolume.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ApplicationVolume resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

