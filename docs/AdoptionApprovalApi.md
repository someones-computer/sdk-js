# AdoptionApprovalApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**adoptionApprovalsDecide**](AdoptionApprovalApi.md#adoptionapprovalsdecide) | **POST** /api/adoption_approvals | Creates a AdoptionApproval resource. |
| [**adoptionApprovalsGet**](AdoptionApprovalApi.md#adoptionapprovalsget) | **GET** /api/adoption_approvals/{id} | Retrieves a AdoptionApproval resource. |
| [**adoptionApprovalsList**](AdoptionApprovalApi.md#adoptionapprovalslist) | **GET** /api/adoption_approvals | Retrieves the collection of AdoptionApproval resources. |
| [**adoptionApprovalsWithdraw**](AdoptionApprovalApi.md#adoptionapprovalswithdraw) | **DELETE** /api/adoption_approvals/{id} | Removes the AdoptionApproval resource. |



## adoptionApprovalsDecide

> AdoptionApproval adoptionApprovalsDecide(adoptionApprovalAdoptionApprovalInput)

Creates a AdoptionApproval resource.

Creates a AdoptionApproval resource.

### Example

```ts
import {
  Configuration,
  AdoptionApprovalApi,
} from '@someones-computer/sdk-js';
import type { AdoptionApprovalsDecideRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdoptionApprovalApi(config);

  const body = {
    // AdoptionApprovalAdoptionApprovalInput | The new AdoptionApproval resource
    adoptionApprovalAdoptionApprovalInput: ...,
  } satisfies AdoptionApprovalsDecideRequest;

  try {
    const data = await api.adoptionApprovalsDecide(body);
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
| **adoptionApprovalAdoptionApprovalInput** | [AdoptionApprovalAdoptionApprovalInput](AdoptionApprovalAdoptionApprovalInput.md) | The new AdoptionApproval resource | |

### Return type

[**AdoptionApproval**](AdoptionApproval.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | AdoptionApproval resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## adoptionApprovalsGet

> AdoptionApproval adoptionApprovalsGet(id)

Retrieves a AdoptionApproval resource.

Retrieves a AdoptionApproval resource.

### Example

```ts
import {
  Configuration,
  AdoptionApprovalApi,
} from '@someones-computer/sdk-js';
import type { AdoptionApprovalsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdoptionApprovalApi(config);

  const body = {
    // string | AdoptionApproval identifier
    id: id_example,
  } satisfies AdoptionApprovalsGetRequest;

  try {
    const data = await api.adoptionApprovalsGet(body);
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
| **id** | `string` | AdoptionApproval identifier | [Defaults to `undefined`] |

### Return type

[**AdoptionApproval**](AdoptionApproval.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AdoptionApproval resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## adoptionApprovalsList

> Array&lt;AdoptionApproval&gt; adoptionApprovalsList(page)

Retrieves the collection of AdoptionApproval resources.

Retrieves the collection of AdoptionApproval resources.

### Example

```ts
import {
  Configuration,
  AdoptionApprovalApi,
} from '@someones-computer/sdk-js';
import type { AdoptionApprovalsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdoptionApprovalApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies AdoptionApprovalsListRequest;

  try {
    const data = await api.adoptionApprovalsList(body);
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

[**Array&lt;AdoptionApproval&gt;**](AdoptionApproval.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AdoptionApproval collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## adoptionApprovalsWithdraw

> adoptionApprovalsWithdraw(id)

Removes the AdoptionApproval resource.

Removes the AdoptionApproval resource.

### Example

```ts
import {
  Configuration,
  AdoptionApprovalApi,
} from '@someones-computer/sdk-js';
import type { AdoptionApprovalsWithdrawRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdoptionApprovalApi(config);

  const body = {
    // string | AdoptionApproval identifier
    id: id_example,
  } satisfies AdoptionApprovalsWithdrawRequest;

  try {
    const data = await api.adoptionApprovalsWithdraw(body);
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
| **id** | `string` | AdoptionApproval identifier | [Defaults to `undefined`] |

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
| **204** | AdoptionApproval resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

