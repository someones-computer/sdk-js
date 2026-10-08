# CreditTransactionApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**creditTransactionsGet**](CreditTransactionApi.md#credittransactionsget) | **GET** /api/credit_transactions/{id} | Retrieves a CreditTransaction resource. |
| [**creditTransactionsList**](CreditTransactionApi.md#credittransactionslist) | **GET** /api/credit_transactions | Retrieves the collection of CreditTransaction resources. |



## creditTransactionsGet

> CreditTransaction creditTransactionsGet(id)

Retrieves a CreditTransaction resource.

Retrieves a CreditTransaction resource.

### Example

```ts
import {
  Configuration,
  CreditTransactionApi,
} from '@someones-computer/sdk-js';
import type { CreditTransactionsGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CreditTransactionApi(config);

  const body = {
    // string | CreditTransaction identifier
    id: id_example,
  } satisfies CreditTransactionsGetRequest;

  try {
    const data = await api.creditTransactionsGet(body);
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
| **id** | `string` | CreditTransaction identifier | [Defaults to `undefined`] |

### Return type

[**CreditTransaction**](CreditTransaction.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CreditTransaction resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## creditTransactionsList

> Array&lt;CreditTransaction&gt; creditTransactionsList(page)

Retrieves the collection of CreditTransaction resources.

Retrieves the collection of CreditTransaction resources.

### Example

```ts
import {
  Configuration,
  CreditTransactionApi,
} from '@someones-computer/sdk-js';
import type { CreditTransactionsListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CreditTransactionApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies CreditTransactionsListRequest;

  try {
    const data = await api.creditTransactionsList(body);
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

[**Array&lt;CreditTransaction&gt;**](CreditTransaction.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CreditTransaction collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

