# OrganizationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**organizationsCreate**](OrganizationApi.md#organizationscreate) | **POST** /api/organizations | Creates a Organization resource. |
| [**organizationsDelete**](OrganizationApi.md#organizationsdelete) | **DELETE** /api/organizations/{id} | Removes the Organization resource. |
| [**organizationsGet**](OrganizationApi.md#organizationsget) | **GET** /api/organizations/{id} | Retrieves a Organization resource. |
| [**organizationsList**](OrganizationApi.md#organizationslist) | **GET** /api/organizations | Retrieves the collection of Organization resources. |
| [**organizationsUpdate**](OrganizationApi.md#organizationsupdate) | **PATCH** /api/organizations/{id} | Updates the Organization resource. |



## organizationsCreate

> Organization organizationsCreate(organization)

Creates a Organization resource.

Creates a Organization resource.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@someones-computer/sdk-js';
import type { OrganizationsCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationApi(config);

  const body = {
    // Organization | The new Organization resource
    organization: ...,
  } satisfies OrganizationsCreateRequest;

  try {
    const data = await api.organizationsCreate(body);
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
| **organization** | [Organization](Organization.md) | The new Organization resource | |

### Return type

[**Organization**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Organization resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## organizationsDelete

> organizationsDelete(id)

Removes the Organization resource.

Removes the Organization resource.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@someones-computer/sdk-js';
import type { OrganizationsDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationApi(config);

  const body = {
    // string | Organization identifier
    id: id_example,
  } satisfies OrganizationsDeleteRequest;

  try {
    const data = await api.organizationsDelete(body);
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
| **id** | `string` | Organization identifier | [Defaults to `undefined`] |

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
| **204** | Organization resource deleted |  -  |
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## organizationsGet

> Organization organizationsGet(id)

Retrieves a Organization resource.

Retrieves a Organization resource.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@someones-computer/sdk-js';
import type { OrganizationsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationApi(config);

  const body = {
    // string | Organization identifier
    id: id_example,
  } satisfies OrganizationsGetRequest;

  try {
    const data = await api.organizationsGet(body);
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
| **id** | `string` | Organization identifier | [Defaults to `undefined`] |

### Return type

[**Organization**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## organizationsList

> Array&lt;Organization&gt; organizationsList(page, slug, slug2)

Retrieves the collection of Organization resources.

Retrieves the collection of Organization resources.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@someones-computer/sdk-js';
import type { OrganizationsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
    // string |  (optional)
    slug: slug_example,
    // Array<string> |  (optional)
    slug2: ...,
  } satisfies OrganizationsListRequest;

  try {
    const data = await api.organizationsList(body);
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

### Return type

[**Array&lt;Organization&gt;**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## organizationsUpdate

> Organization organizationsUpdate(id, organizationJsonMergePatch)

Updates the Organization resource.

Updates the Organization resource.

### Example

```ts
import {
  Configuration,
  OrganizationApi,
} from '@someones-computer/sdk-js';
import type { OrganizationsUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationApi(config);

  const body = {
    // string | Organization identifier
    id: id_example,
    // OrganizationJsonMergePatch | The updated Organization resource
    organizationJsonMergePatch: ...,
  } satisfies OrganizationsUpdateRequest;

  try {
    const data = await api.organizationsUpdate(body);
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
| **id** | `string` | Organization identifier | [Defaults to `undefined`] |
| **organizationJsonMergePatch** | [OrganizationJsonMergePatch](OrganizationJsonMergePatch.md) | The updated Organization resource | |

### Return type

[**Organization**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

