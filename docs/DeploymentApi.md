# DeploymentApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deploymentsBundleUploadConfirm**](DeploymentApi.md#deploymentsbundleuploadconfirm) | **POST** /api/deployments/bundle_uploads/confirm | Creates a Deployment resource. |
| [**deploymentsBundleUploadDeclare**](DeploymentApi.md#deploymentsbundleuploaddeclare) | **POST** /api/deployments/bundle_uploads | Creates a Deployment resource. |
| [**deploymentsCreate**](DeploymentApi.md#deploymentscreate) | **POST** /api/deployments | Creates a Deployment resource. |
| [**deploymentsDelete**](DeploymentApi.md#deploymentsdelete) | **DELETE** /api/deployments/{id} | Removes the Deployment resource. |
| [**deploymentsEndpoints**](DeploymentApi.md#deploymentsendpoints) | **GET** /api/deployments/{id}/endpoints | Retrieves the collection of Deployment resources. |
| [**deploymentsGet**](DeploymentApi.md#deploymentsget) | **GET** /api/deployments/{id} | Retrieves a Deployment resource. |
| [**deploymentsList**](DeploymentApi.md#deploymentslist) | **GET** /api/deployments | Retrieves the collection of Deployment resources. |
| [**deploymentsUpdate**](DeploymentApi.md#deploymentsupdate) | **PATCH** /api/deployments/{id} | Updates the Deployment resource. |



## deploymentsBundleUploadConfirm

> DeploymentBundleUploadConfirmOutput deploymentsBundleUploadConfirm(deploymentBundleUploadConfirmInput)

Creates a Deployment resource.

Creates a Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsBundleUploadConfirmRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // DeploymentBundleUploadConfirmInput | The new Deployment resource
    deploymentBundleUploadConfirmInput: ...,
  } satisfies DeploymentsBundleUploadConfirmRequest;

  try {
    const data = await api.deploymentsBundleUploadConfirm(body);
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
| **deploymentBundleUploadConfirmInput** | [DeploymentBundleUploadConfirmInput](DeploymentBundleUploadConfirmInput.md) | The new Deployment resource | |

### Return type

[**DeploymentBundleUploadConfirmOutput**](DeploymentBundleUploadConfirmOutput.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsBundleUploadDeclare

> DeploymentBundleUploadDeclareOutput deploymentsBundleUploadDeclare(deploymentBundleUploadDeclareInput)

Creates a Deployment resource.

Creates a Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsBundleUploadDeclareRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // DeploymentBundleUploadDeclareInput | The new Deployment resource
    deploymentBundleUploadDeclareInput: ...,
  } satisfies DeploymentsBundleUploadDeclareRequest;

  try {
    const data = await api.deploymentsBundleUploadDeclare(body);
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
| **deploymentBundleUploadDeclareInput** | [DeploymentBundleUploadDeclareInput](DeploymentBundleUploadDeclareInput.md) | The new Deployment resource | |

### Return type

[**DeploymentBundleUploadDeclareOutput**](DeploymentBundleUploadDeclareOutput.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsCreate

> Deployment deploymentsCreate(deployment)

Creates a Deployment resource.

Creates a Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // Deployment | The new Deployment resource
    deployment: ...,
  } satisfies DeploymentsCreateRequest;

  try {
    const data = await api.deploymentsCreate(body);
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
| **deployment** | [Deployment](Deployment.md) | The new Deployment resource | |

### Return type

[**Deployment**](Deployment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Deployment resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsDelete

> deploymentsDelete(id)

Removes the Deployment resource.

Removes the Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // string | Deployment identifier
    id: id_example,
  } satisfies DeploymentsDeleteRequest;

  try {
    const data = await api.deploymentsDelete(body);
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
| **id** | `string` | Deployment identifier | [Defaults to `undefined`] |

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
| **204** | Deployment resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsEndpoints

> Array&lt;DeploymentDeploymentEndpoint&gt; deploymentsEndpoints(id)

Retrieves the collection of Deployment resources.

Retrieves the collection of Deployment resources.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsEndpointsRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // string | Deployment identifier
    id: id_example,
  } satisfies DeploymentsEndpointsRequest;

  try {
    const data = await api.deploymentsEndpoints(body);
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
| **id** | `string` | Deployment identifier | [Defaults to `undefined`] |

### Return type

[**Array&lt;DeploymentDeploymentEndpoint&gt;**](DeploymentDeploymentEndpoint.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsGet

> Deployment deploymentsGet(id)

Retrieves a Deployment resource.

Retrieves a Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // string | Deployment identifier
    id: id_example,
  } satisfies DeploymentsGetRequest;

  try {
    const data = await api.deploymentsGet(body);
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
| **id** | `string` | Deployment identifier | [Defaults to `undefined`] |

### Return type

[**Deployment**](Deployment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsList

> Array&lt;Deployment&gt; deploymentsList(page, application, application2, sequence, sequence2, name, name2, itemsPerPage)

Retrieves the collection of Deployment resources.

Retrieves the collection of Deployment resources.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
    // string | Only revisions of this application, by IRI (`/api/applications/{id}`). (optional)
    application: application_example,
    // Array<string> | Only revisions of this application, by IRI (`/api/applications/{id}`). (optional)
    application2: ...,
    // string | Only the revision with this sequence number. (optional)
    sequence: sequence_example,
    // Array<string> | Only the revision with this sequence number. (optional)
    sequence2: ...,
    // string | Only revisions with this exact name. (optional)
    name: name_example,
    // Array<string> | Only revisions with this exact name. (optional)
    name2: ...,
    // string | Rows per page. (optional)
    itemsPerPage: itemsPerPage_example,
  } satisfies DeploymentsListRequest;

  try {
    const data = await api.deploymentsList(body);
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
| **application** | `string` | Only revisions of this application, by IRI (&#x60;/api/applications/{id}&#x60;). | [Optional] [Defaults to `undefined`] |
| **application2** | `Array<string>` | Only revisions of this application, by IRI (&#x60;/api/applications/{id}&#x60;). | [Optional] |
| **sequence** | `string` | Only the revision with this sequence number. | [Optional] [Defaults to `undefined`] |
| **sequence2** | `Array<string>` | Only the revision with this sequence number. | [Optional] |
| **name** | `string` | Only revisions with this exact name. | [Optional] [Defaults to `undefined`] |
| **name2** | `Array<string>` | Only revisions with this exact name. | [Optional] |
| **itemsPerPage** | `string` | Rows per page. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Deployment&gt;**](Deployment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deploymentsUpdate

> Deployment deploymentsUpdate(id, deploymentJsonMergePatch)

Updates the Deployment resource.

Updates the Deployment resource.

### Example

```ts
import {
  Configuration,
  DeploymentApi,
} from '@someones-computer/sdk-js';
import type { DeploymentsUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeploymentApi(config);

  const body = {
    // string | Deployment identifier
    id: id_example,
    // DeploymentJsonMergePatch | The updated Deployment resource
    deploymentJsonMergePatch: ...,
  } satisfies DeploymentsUpdateRequest;

  try {
    const data = await api.deploymentsUpdate(body);
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
| **id** | `string` | Deployment identifier | [Defaults to `undefined`] |
| **deploymentJsonMergePatch** | [DeploymentJsonMergePatch](DeploymentJsonMergePatch.md) | The updated Deployment resource | |

### Return type

[**Deployment**](Deployment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deployment resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

