# ServiceBindingApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**serviceBindingsCreate**](ServiceBindingApi.md#servicebindingscreate) | **POST** /api/service_bindings | Creates a ServiceBinding resource. |
| [**serviceBindingsDelete**](ServiceBindingApi.md#servicebindingsdelete) | **DELETE** /api/service_bindings/{id} | Removes the ServiceBinding resource. |
| [**serviceBindingsGet**](ServiceBindingApi.md#servicebindingsget) | **GET** /api/service_bindings/{id} | Retrieves a ServiceBinding resource. |
| [**serviceBindingsList**](ServiceBindingApi.md#servicebindingslist) | **GET** /api/service_bindings | Retrieves the collection of ServiceBinding resources. |



## serviceBindingsCreate

> ServiceBinding serviceBindingsCreate(serviceBindingServiceBindingInput)

Creates a ServiceBinding resource.

Creates a ServiceBinding resource.

### Example

```ts
import {
  Configuration,
  ServiceBindingApi,
} from '@someones-computer/sdk-js';
import type { ServiceBindingsCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceBindingApi(config);

  const body = {
    // ServiceBindingServiceBindingInput | The new ServiceBinding resource
    serviceBindingServiceBindingInput: ...,
  } satisfies ServiceBindingsCreateRequest;

  try {
    const data = await api.serviceBindingsCreate(body);
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
| **serviceBindingServiceBindingInput** | [ServiceBindingServiceBindingInput](ServiceBindingServiceBindingInput.md) | The new ServiceBinding resource | |

### Return type

[**ServiceBinding**](ServiceBinding.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | ServiceBinding resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## serviceBindingsDelete

> serviceBindingsDelete(id)

Removes the ServiceBinding resource.

Removes the ServiceBinding resource.

### Example

```ts
import {
  Configuration,
  ServiceBindingApi,
} from '@someones-computer/sdk-js';
import type { ServiceBindingsDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceBindingApi(config);

  const body = {
    // string | ServiceBinding identifier
    id: id_example,
  } satisfies ServiceBindingsDeleteRequest;

  try {
    const data = await api.serviceBindingsDelete(body);
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
| **id** | `string` | ServiceBinding identifier | [Defaults to `undefined`] |

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
| **204** | ServiceBinding resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## serviceBindingsGet

> ServiceBinding serviceBindingsGet(id)

Retrieves a ServiceBinding resource.

Retrieves a ServiceBinding resource.

### Example

```ts
import {
  Configuration,
  ServiceBindingApi,
} from '@someones-computer/sdk-js';
import type { ServiceBindingsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceBindingApi(config);

  const body = {
    // string | ServiceBinding identifier
    id: id_example,
  } satisfies ServiceBindingsGetRequest;

  try {
    const data = await api.serviceBindingsGet(body);
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
| **id** | `string` | ServiceBinding identifier | [Defaults to `undefined`] |

### Return type

[**ServiceBinding**](ServiceBinding.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ServiceBinding resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## serviceBindingsList

> Array&lt;ServiceBinding&gt; serviceBindingsList(page)

Retrieves the collection of ServiceBinding resources.

Retrieves the collection of ServiceBinding resources.

### Example

```ts
import {
  Configuration,
  ServiceBindingApi,
} from '@someones-computer/sdk-js';
import type { ServiceBindingsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceBindingApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies ServiceBindingsListRequest;

  try {
    const data = await api.serviceBindingsList(body);
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

[**Array&lt;ServiceBinding&gt;**](ServiceBinding.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ServiceBinding collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

