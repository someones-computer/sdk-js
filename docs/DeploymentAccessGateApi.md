# DeploymentAccessGateApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deploymentAccessGatesCreate**](DeploymentAccessGateApi.md#deploymentaccessgatescreate) | **POST** /api/deployment_access_gates | Creates a DeploymentAccessGate resource. |
| [**deploymentAccessGatesDelete**](DeploymentAccessGateApi.md#deploymentaccessgatesdelete) | **DELETE** /api/deployment_access_gates/{id} | Removes the DeploymentAccessGate resource. |
| [**deploymentAccessGatesGet**](DeploymentAccessGateApi.md#deploymentaccessgatesget) | **GET** /api/deployment_access_gates/{id} | Retrieves a DeploymentAccessGate resource. |
| [**deploymentAccessGatesList**](DeploymentAccessGateApi.md#deploymentaccessgateslist) | **GET** /api/deployment_access_gates | Retrieves the collection of DeploymentAccessGate resources. |
| [**deploymentAccessGatesUpdate**](DeploymentAccessGateApi.md#deploymentaccessgatesupdate) | **PATCH** /api/deployment_access_gates/{id} | Updates the DeploymentAccessGate resource. |



## deploymentAccessGatesCreate

> DeploymentAccessGate deploymentAccessGatesCreate(deploymentAccessGate)

Creates a DeploymentAccessGate resource.

Creates a DeploymentAccessGate resource.

### Example

```ts
import {
  Configuration,
  DeploymentAccessGateApi,
} from '@someones-computer/sdk-js';
import type { DeploymentAccessGatesCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentAccessGateApi(config);

  const body = {
    // DeploymentAccessGate | The new DeploymentAccessGate resource
    deploymentAccessGate: ...,
  } satisfies DeploymentAccessGatesCreateRequest;

  try {
    const data = await api.deploymentAccessGatesCreate(body);
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
| **deploymentAccessGate** | [DeploymentAccessGate](DeploymentAccessGate.md) | The new DeploymentAccessGate resource | |

### Return type

[**DeploymentAccessGate**](DeploymentAccessGate.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | DeploymentAccessGate resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentAccessGatesDelete

> deploymentAccessGatesDelete(id)

Removes the DeploymentAccessGate resource.

Removes the DeploymentAccessGate resource.

### Example

```ts
import {
  Configuration,
  DeploymentAccessGateApi,
} from '@someones-computer/sdk-js';
import type { DeploymentAccessGatesDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentAccessGateApi(config);

  const body = {
    // string | DeploymentAccessGate identifier
    id: id_example,
  } satisfies DeploymentAccessGatesDeleteRequest;

  try {
    const data = await api.deploymentAccessGatesDelete(body);
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
| **id** | `string` | DeploymentAccessGate identifier | [Defaults to `undefined`] |

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
| **204** | DeploymentAccessGate resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentAccessGatesGet

> DeploymentAccessGate deploymentAccessGatesGet(id)

Retrieves a DeploymentAccessGate resource.

Retrieves a DeploymentAccessGate resource.

### Example

```ts
import {
  Configuration,
  DeploymentAccessGateApi,
} from '@someones-computer/sdk-js';
import type { DeploymentAccessGatesGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentAccessGateApi(config);

  const body = {
    // string | DeploymentAccessGate identifier
    id: id_example,
  } satisfies DeploymentAccessGatesGetRequest;

  try {
    const data = await api.deploymentAccessGatesGet(body);
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
| **id** | `string` | DeploymentAccessGate identifier | [Defaults to `undefined`] |

### Return type

[**DeploymentAccessGate**](DeploymentAccessGate.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DeploymentAccessGate resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentAccessGatesList

> Array&lt;DeploymentAccessGate&gt; deploymentAccessGatesList(page)

Retrieves the collection of DeploymentAccessGate resources.

Retrieves the collection of DeploymentAccessGate resources.

### Example

```ts
import {
  Configuration,
  DeploymentAccessGateApi,
} from '@someones-computer/sdk-js';
import type { DeploymentAccessGatesListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentAccessGateApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies DeploymentAccessGatesListRequest;

  try {
    const data = await api.deploymentAccessGatesList(body);
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

[**Array&lt;DeploymentAccessGate&gt;**](DeploymentAccessGate.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DeploymentAccessGate collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentAccessGatesUpdate

> DeploymentAccessGate deploymentAccessGatesUpdate(id, deploymentAccessGateJsonMergePatch)

Updates the DeploymentAccessGate resource.

Updates the DeploymentAccessGate resource.

### Example

```ts
import {
  Configuration,
  DeploymentAccessGateApi,
} from '@someones-computer/sdk-js';
import type { DeploymentAccessGatesUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentAccessGateApi(config);

  const body = {
    // string | DeploymentAccessGate identifier
    id: id_example,
    // DeploymentAccessGateJsonMergePatch | The updated DeploymentAccessGate resource
    deploymentAccessGateJsonMergePatch: ...,
  } satisfies DeploymentAccessGatesUpdateRequest;

  try {
    const data = await api.deploymentAccessGatesUpdate(body);
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
| **id** | `string` | DeploymentAccessGate identifier | [Defaults to `undefined`] |
| **deploymentAccessGateJsonMergePatch** | [DeploymentAccessGateJsonMergePatch](DeploymentAccessGateJsonMergePatch.md) | The updated DeploymentAccessGate resource | |

### Return type

[**DeploymentAccessGate**](DeploymentAccessGate.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DeploymentAccessGate resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

