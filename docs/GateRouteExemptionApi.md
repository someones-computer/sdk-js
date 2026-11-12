# GateRouteExemptionApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiGateRouteExemptionsGetCollection**](GateRouteExemptionApi.md#apigaterouteexemptionsgetcollection) | **GET** /api/gate_route_exemptions | Retrieves the collection of GateRouteExemption resources. |
| [**apiGateRouteExemptionsIdDelete**](GateRouteExemptionApi.md#apigaterouteexemptionsiddelete) | **DELETE** /api/gate_route_exemptions/{id} | Removes the GateRouteExemption resource. |
| [**apiGateRouteExemptionsIdGet**](GateRouteExemptionApi.md#apigaterouteexemptionsidget) | **GET** /api/gate_route_exemptions/{id} | Retrieves a GateRouteExemption resource. |
| [**apiGateRouteExemptionsPost**](GateRouteExemptionApi.md#apigaterouteexemptionspost) | **POST** /api/gate_route_exemptions | Creates a GateRouteExemption resource. |



## apiGateRouteExemptionsGetCollection

> Array&lt;GateRouteExemption&gt; apiGateRouteExemptionsGetCollection(page)

Retrieves the collection of GateRouteExemption resources.

Retrieves the collection of GateRouteExemption resources.

### Example

```ts
import {
  Configuration,
  GateRouteExemptionApi,
} from '@someones-computer/sdk-js';
import type { ApiGateRouteExemptionsGetCollectionRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GateRouteExemptionApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies ApiGateRouteExemptionsGetCollectionRequest;

  try {
    const data = await api.apiGateRouteExemptionsGetCollection(body);
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

[**Array&lt;GateRouteExemption&gt;**](GateRouteExemption.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GateRouteExemption collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiGateRouteExemptionsIdDelete

> apiGateRouteExemptionsIdDelete(id)

Removes the GateRouteExemption resource.

Removes the GateRouteExemption resource.

### Example

```ts
import {
  Configuration,
  GateRouteExemptionApi,
} from '@someones-computer/sdk-js';
import type { ApiGateRouteExemptionsIdDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GateRouteExemptionApi(config);

  const body = {
    // string | GateRouteExemption identifier
    id: id_example,
  } satisfies ApiGateRouteExemptionsIdDeleteRequest;

  try {
    const data = await api.apiGateRouteExemptionsIdDelete(body);
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
| **id** | `string` | GateRouteExemption identifier | [Defaults to `undefined`] |

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
| **204** | GateRouteExemption resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiGateRouteExemptionsIdGet

> GateRouteExemption apiGateRouteExemptionsIdGet(id)

Retrieves a GateRouteExemption resource.

Retrieves a GateRouteExemption resource.

### Example

```ts
import {
  Configuration,
  GateRouteExemptionApi,
} from '@someones-computer/sdk-js';
import type { ApiGateRouteExemptionsIdGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GateRouteExemptionApi(config);

  const body = {
    // string | GateRouteExemption identifier
    id: id_example,
  } satisfies ApiGateRouteExemptionsIdGetRequest;

  try {
    const data = await api.apiGateRouteExemptionsIdGet(body);
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
| **id** | `string` | GateRouteExemption identifier | [Defaults to `undefined`] |

### Return type

[**GateRouteExemption**](GateRouteExemption.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GateRouteExemption resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiGateRouteExemptionsPost

> GateRouteExemption apiGateRouteExemptionsPost(gateRouteExemptionGateRouteExemptionInput)

Creates a GateRouteExemption resource.

Creates a GateRouteExemption resource.

### Example

```ts
import {
  Configuration,
  GateRouteExemptionApi,
} from '@someones-computer/sdk-js';
import type { ApiGateRouteExemptionsPostRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GateRouteExemptionApi(config);

  const body = {
    // GateRouteExemptionGateRouteExemptionInput | The new GateRouteExemption resource
    gateRouteExemptionGateRouteExemptionInput: ...,
  } satisfies ApiGateRouteExemptionsPostRequest;

  try {
    const data = await api.apiGateRouteExemptionsPost(body);
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
| **gateRouteExemptionGateRouteExemptionInput** | [GateRouteExemptionGateRouteExemptionInput](GateRouteExemptionGateRouteExemptionInput.md) | The new GateRouteExemption resource | |

### Return type

[**GateRouteExemption**](GateRouteExemption.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | GateRouteExemption resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

