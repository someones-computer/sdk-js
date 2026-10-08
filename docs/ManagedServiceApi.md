# ManagedServiceApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**managedServicesCreate**](ManagedServiceApi.md#managedservicescreate) | **POST** /api/managed_services | Creates a ManagedService resource. |
| [**managedServicesDelete**](ManagedServiceApi.md#managedservicesdelete) | **DELETE** /api/managed_services/{id} | Removes the ManagedService resource. |
| [**managedServicesGet**](ManagedServiceApi.md#managedservicesget) | **GET** /api/managed_services/{id} | Retrieves a ManagedService resource. |
| [**managedServicesList**](ManagedServiceApi.md#managedserviceslist) | **GET** /api/managed_services | Retrieves the collection of ManagedService resources. |
| [**managedServicesListRetired**](ManagedServiceApi.md#managedserviceslistretired) | **GET** /api/managed_services/retired | Retrieves the collection of ManagedService resources. |
| [**managedServicesRestore**](ManagedServiceApi.md#managedservicesrestore) | **POST** /api/managed_services/{id}/restore | Creates a ManagedService resource. |
| [**managedServicesResume**](ManagedServiceApi.md#managedservicesresume) | **POST** /api/managed_services/{id}/resume | Creates a ManagedService resource. |
| [**managedServicesSuspend**](ManagedServiceApi.md#managedservicessuspend) | **POST** /api/managed_services/{id}/suspend | Creates a ManagedService resource. |



## managedServicesCreate

> ManagedService managedServicesCreate(managedServiceManagedServiceInput)

Creates a ManagedService resource.

Creates a ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // ManagedServiceManagedServiceInput | The new ManagedService resource
    managedServiceManagedServiceInput: ...,
  } satisfies ManagedServicesCreateRequest;

  try {
    const data = await api.managedServicesCreate(body);
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
| **managedServiceManagedServiceInput** | [ManagedServiceManagedServiceInput](ManagedServiceManagedServiceInput.md) | The new ManagedService resource | |

### Return type

[**ManagedService**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | ManagedService resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesDelete

> managedServicesDelete(id)

Removes the ManagedService resource.

Removes the ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // string | ManagedService identifier
    id: id_example,
  } satisfies ManagedServicesDeleteRequest;

  try {
    const data = await api.managedServicesDelete(body);
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
| **id** | `string` | ManagedService identifier | [Defaults to `undefined`] |

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
| **204** | ManagedService resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesGet

> ManagedService managedServicesGet(id)

Retrieves a ManagedService resource.

Retrieves a ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // string | ManagedService identifier
    id: id_example,
  } satisfies ManagedServicesGetRequest;

  try {
    const data = await api.managedServicesGet(body);
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
| **id** | `string` | ManagedService identifier | [Defaults to `undefined`] |

### Return type

[**ManagedService**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesList

> Array&lt;ManagedService&gt; managedServicesList(page)

Retrieves the collection of ManagedService resources.

Retrieves the collection of ManagedService resources.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies ManagedServicesListRequest;

  try {
    const data = await api.managedServicesList(body);
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

[**Array&lt;ManagedService&gt;**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesListRetired

> Array&lt;ManagedService&gt; managedServicesListRetired()

Retrieves the collection of ManagedService resources.

Retrieves the collection of ManagedService resources.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesListRetiredRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  try {
    const data = await api.managedServicesListRetired();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;ManagedService&gt;**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesRestore

> ManagedService managedServicesRestore(id)

Creates a ManagedService resource.

Creates a ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesRestoreRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // string | ManagedService identifier
    id: id_example,
  } satisfies ManagedServicesRestoreRequest;

  try {
    const data = await api.managedServicesRestore(body);
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
| **id** | `string` | ManagedService identifier | [Defaults to `undefined`] |

### Return type

[**ManagedService**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesResume

> ManagedService managedServicesResume(id)

Creates a ManagedService resource.

Creates a ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesResumeRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // string | ManagedService identifier
    id: id_example,
  } satisfies ManagedServicesResumeRequest;

  try {
    const data = await api.managedServicesResume(body);
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
| **id** | `string` | ManagedService identifier | [Defaults to `undefined`] |

### Return type

[**ManagedService**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## managedServicesSuspend

> ManagedService managedServicesSuspend(id)

Creates a ManagedService resource.

Creates a ManagedService resource.

### Example

```ts
import {
  Configuration,
  ManagedServiceApi,
} from '@someones-computer/sdk-js';
import type { ManagedServicesSuspendRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ManagedServiceApi(config);

  const body = {
    // string | ManagedService identifier
    id: id_example,
  } satisfies ManagedServicesSuspendRequest;

  try {
    const data = await api.managedServicesSuspend(body);
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
| **id** | `string` | ManagedService identifier | [Defaults to `undefined`] |

### Return type

[**ManagedService**](ManagedService.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ManagedService resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

