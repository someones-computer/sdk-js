# VolumeApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**volumesCreate**](VolumeApi.md#volumescreate) | **POST** /api/volumes | Creates a Volume resource. |
| [**volumesDelete**](VolumeApi.md#volumesdelete) | **DELETE** /api/volumes/{id} | Removes the Volume resource. |
| [**volumesGet**](VolumeApi.md#volumesget) | **GET** /api/volumes/{id} | Retrieves a Volume resource. |
| [**volumesList**](VolumeApi.md#volumeslist) | **GET** /api/volumes | Retrieves the collection of Volume resources. |



## volumesCreate

> Volume volumesCreate(volumeVolumeInput)

Creates a Volume resource.

Creates a Volume resource.

### Example

```ts
import {
  Configuration,
  VolumeApi,
} from '@someones-computer/sdk-js';
import type { VolumesCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VolumeApi(config);

  const body = {
    // VolumeVolumeInput | The new Volume resource
    volumeVolumeInput: ...,
  } satisfies VolumesCreateRequest;

  try {
    const data = await api.volumesCreate(body);
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
| **volumeVolumeInput** | [VolumeVolumeInput](VolumeVolumeInput.md) | The new Volume resource | |

### Return type

[**Volume**](Volume.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Volume resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## volumesDelete

> volumesDelete(id)

Removes the Volume resource.

Removes the Volume resource.

### Example

```ts
import {
  Configuration,
  VolumeApi,
} from '@someones-computer/sdk-js';
import type { VolumesDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VolumeApi(config);

  const body = {
    // string | Volume identifier
    id: id_example,
  } satisfies VolumesDeleteRequest;

  try {
    const data = await api.volumesDelete(body);
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
| **id** | `string` | Volume identifier | [Defaults to `undefined`] |

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
| **204** | Volume resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## volumesGet

> Volume volumesGet(id)

Retrieves a Volume resource.

Retrieves a Volume resource.

### Example

```ts
import {
  Configuration,
  VolumeApi,
} from '@someones-computer/sdk-js';
import type { VolumesGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VolumeApi(config);

  const body = {
    // string | Volume identifier
    id: id_example,
  } satisfies VolumesGetRequest;

  try {
    const data = await api.volumesGet(body);
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
| **id** | `string` | Volume identifier | [Defaults to `undefined`] |

### Return type

[**Volume**](Volume.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Volume resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## volumesList

> Array&lt;Volume&gt; volumesList(page)

Retrieves the collection of Volume resources.

Retrieves the collection of Volume resources.

### Example

```ts
import {
  Configuration,
  VolumeApi,
} from '@someones-computer/sdk-js';
import type { VolumesListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VolumeApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies VolumesListRequest;

  try {
    const data = await api.volumesList(body);
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

[**Array&lt;Volume&gt;**](Volume.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Volume collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

