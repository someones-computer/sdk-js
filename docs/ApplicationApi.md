# ApplicationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**applicationsCreate**](ApplicationApi.md#applicationscreate) | **POST** /api/applications | Creates a Application resource. |
| [**applicationsDelete**](ApplicationApi.md#applicationsdelete) | **DELETE** /api/applications/{id} | Removes the Application resource. |
| [**applicationsGet**](ApplicationApi.md#applicationsget) | **GET** /api/applications/{id} | Retrieves a Application resource. |
| [**applicationsList**](ApplicationApi.md#applicationslist) | **GET** /api/applications | Retrieves the collection of Application resources. |
| [**applicationsUpdate**](ApplicationApi.md#applicationsupdate) | **PATCH** /api/applications/{id} | Updates the Application resource. |



## applicationsCreate

> Application applicationsCreate(application)

Creates a Application resource.

Creates a Application resource.

### Example

```ts
import {
  Configuration,
  ApplicationApi,
} from '@someones-computer/sdk-js';
import type { ApplicationsCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationApi(config);

  const body = {
    // Application | The new Application resource
    application: ...,
  } satisfies ApplicationsCreateRequest;

  try {
    const data = await api.applicationsCreate(body);
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
| **application** | [Application](Application.md) | The new Application resource | |

### Return type

[**Application**](Application.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Application resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## applicationsDelete

> applicationsDelete(id)

Removes the Application resource.

Removes the Application resource.

### Example

```ts
import {
  Configuration,
  ApplicationApi,
} from '@someones-computer/sdk-js';
import type { ApplicationsDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationApi(config);

  const body = {
    // string | Application identifier
    id: id_example,
  } satisfies ApplicationsDeleteRequest;

  try {
    const data = await api.applicationsDelete(body);
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
| **id** | `string` | Application identifier | [Defaults to `undefined`] |

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
| **204** | Application resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## applicationsGet

> Application applicationsGet(id)

Retrieves a Application resource.

Retrieves a Application resource.

### Example

```ts
import {
  Configuration,
  ApplicationApi,
} from '@someones-computer/sdk-js';
import type { ApplicationsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationApi(config);

  const body = {
    // string | Application identifier
    id: id_example,
  } satisfies ApplicationsGetRequest;

  try {
    const data = await api.applicationsGet(body);
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
| **id** | `string` | Application identifier | [Defaults to `undefined`] |

### Return type

[**Application**](Application.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Application resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## applicationsList

> Array&lt;Application&gt; applicationsList(page, slug, slug2, organization, organization2, organizationSlug, organizationSlug2)

Retrieves the collection of Application resources.

Retrieves the collection of Application resources.

### Example

```ts
import {
  Configuration,
  ApplicationApi,
} from '@someones-computer/sdk-js';
import type { ApplicationsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
    // string |  (optional)
    slug: slug_example,
    // Array<string> |  (optional)
    slug2: ...,
    // string |  (optional)
    organization: organization_example,
    // Array<string> |  (optional)
    organization2: ...,
    // string |  (optional)
    organizationSlug: organizationSlug_example,
    // Array<string> |  (optional)
    organizationSlug2: ...,
  } satisfies ApplicationsListRequest;

  try {
    const data = await api.applicationsList(body);
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
| **slug** | `string` |  | [Optional] [Defaults to `undefined`] |
| **slug2** | `Array<string>` |  | [Optional] |
| **organization** | `string` |  | [Optional] [Defaults to `undefined`] |
| **organization2** | `Array<string>` |  | [Optional] |
| **organizationSlug** | `string` |  | [Optional] [Defaults to `undefined`] |
| **organizationSlug2** | `Array<string>` |  | [Optional] |

### Return type

[**Array&lt;Application&gt;**](Application.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Application collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## applicationsUpdate

> Application applicationsUpdate(id, applicationJsonMergePatch)

Updates the Application resource.

Updates the Application resource.

### Example

```ts
import {
  Configuration,
  ApplicationApi,
} from '@someones-computer/sdk-js';
import type { ApplicationsUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ApplicationApi(config);

  const body = {
    // string | Application identifier
    id: id_example,
    // ApplicationJsonMergePatch | The updated Application resource
    applicationJsonMergePatch: ...,
  } satisfies ApplicationsUpdateRequest;

  try {
    const data = await api.applicationsUpdate(body);
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
| **id** | `string` | Application identifier | [Defaults to `undefined`] |
| **applicationJsonMergePatch** | [ApplicationJsonMergePatch](ApplicationJsonMergePatch.md) | The updated Application resource | |

### Return type

[**Application**](Application.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Application resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

