# SwarmApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**swarmsCreate**](SwarmApi.md#swarmscreate) | **POST** /api/swarms | Creates a Swarm resource. |
| [**swarmsDelete**](SwarmApi.md#swarmsdelete) | **DELETE** /api/swarms/{id} | Removes the Swarm resource. |
| [**swarmsGet**](SwarmApi.md#swarmsget) | **GET** /api/swarms/{id} | Retrieves a Swarm resource. |
| [**swarmsList**](SwarmApi.md#swarmslist) | **GET** /api/swarms | Retrieves the collection of Swarm resources. |
| [**swarmsUpdate**](SwarmApi.md#swarmsupdate) | **PATCH** /api/swarms/{id} | Updates the Swarm resource. |



## swarmsCreate

> Swarm swarmsCreate(swarm)

Creates a Swarm resource.

Creates a Swarm resource.

### Example

```ts
import {
  Configuration,
  SwarmApi,
} from '@someones-computer/sdk-js';
import type { SwarmsCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SwarmApi(config);

  const body = {
    // Swarm | The new Swarm resource
    swarm: ...,
  } satisfies SwarmsCreateRequest;

  try {
    const data = await api.swarmsCreate(body);
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
| **swarm** | [Swarm](Swarm.md) | The new Swarm resource | |

### Return type

[**Swarm**](Swarm.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Swarm resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## swarmsDelete

> swarmsDelete(id)

Removes the Swarm resource.

Removes the Swarm resource.

### Example

```ts
import {
  Configuration,
  SwarmApi,
} from '@someones-computer/sdk-js';
import type { SwarmsDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SwarmApi(config);

  const body = {
    // string | Swarm identifier
    id: id_example,
  } satisfies SwarmsDeleteRequest;

  try {
    const data = await api.swarmsDelete(body);
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
| **id** | `string` | Swarm identifier | [Defaults to `undefined`] |

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
| **204** | Swarm resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## swarmsGet

> Swarm swarmsGet(id)

Retrieves a Swarm resource.

Retrieves a Swarm resource.

### Example

```ts
import {
  Configuration,
  SwarmApi,
} from '@someones-computer/sdk-js';
import type { SwarmsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SwarmApi(config);

  const body = {
    // string | Swarm identifier
    id: id_example,
  } satisfies SwarmsGetRequest;

  try {
    const data = await api.swarmsGet(body);
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
| **id** | `string` | Swarm identifier | [Defaults to `undefined`] |

### Return type

[**Swarm**](Swarm.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Swarm resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## swarmsList

> Array&lt;Swarm&gt; swarmsList(page)

Retrieves the collection of Swarm resources.

Retrieves the collection of Swarm resources.

### Example

```ts
import {
  Configuration,
  SwarmApi,
} from '@someones-computer/sdk-js';
import type { SwarmsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SwarmApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies SwarmsListRequest;

  try {
    const data = await api.swarmsList(body);
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

[**Array&lt;Swarm&gt;**](Swarm.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Swarm collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## swarmsUpdate

> Swarm swarmsUpdate(id, swarmJsonMergePatch)

Updates the Swarm resource.

Updates the Swarm resource.

### Example

```ts
import {
  Configuration,
  SwarmApi,
} from '@someones-computer/sdk-js';
import type { SwarmsUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SwarmApi(config);

  const body = {
    // string | Swarm identifier
    id: id_example,
    // SwarmJsonMergePatch | The updated Swarm resource
    swarmJsonMergePatch: ...,
  } satisfies SwarmsUpdateRequest;

  try {
    const data = await api.swarmsUpdate(body);
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
| **id** | `string` | Swarm identifier | [Defaults to `undefined`] |
| **swarmJsonMergePatch** | [SwarmJsonMergePatch](SwarmJsonMergePatch.md) | The updated Swarm resource | |

### Return type

[**Swarm**](Swarm.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Swarm resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

