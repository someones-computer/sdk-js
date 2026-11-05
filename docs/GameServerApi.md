# GameServerApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**gameServersCreate**](GameServerApi.md#gameserverscreate) | **POST** /api/game_servers | Creates a GameServer resource. |
| [**gameServersDelete**](GameServerApi.md#gameserversdelete) | **DELETE** /api/game_servers/{id} | Removes the GameServer resource. |
| [**gameServersGet**](GameServerApi.md#gameserversget) | **GET** /api/game_servers/{id} | Retrieves a GameServer resource. |
| [**gameServersList**](GameServerApi.md#gameserverslist) | **GET** /api/game_servers | Retrieves the collection of GameServer resources. |
| [**gameServersRestart**](GameServerApi.md#gameserversrestart) | **POST** /api/game_servers/{id}/restart | Creates a GameServer resource. |
| [**gameServersStart**](GameServerApi.md#gameserversstart) | **POST** /api/game_servers/{id}/start | Creates a GameServer resource. |
| [**gameServersStop**](GameServerApi.md#gameserversstop) | **POST** /api/game_servers/{id}/stop | Creates a GameServer resource. |
| [**gameServersUpdate**](GameServerApi.md#gameserversupdate) | **PATCH** /api/game_servers/{id} | Updates the GameServer resource. |



## gameServersCreate

> GameServerGameServerRead gameServersCreate(gameServerGameServerInput)

Creates a GameServer resource.

Creates a GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersCreateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // GameServerGameServerInput | The new GameServer resource
    gameServerGameServerInput: ...,
  } satisfies GameServersCreateRequest;

  try {
    const data = await api.gameServersCreate(body);
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
| **gameServerGameServerInput** | [GameServerGameServerInput](GameServerGameServerInput.md) | The new GameServer resource | |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | GameServer resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersDelete

> gameServersDelete(id)

Removes the GameServer resource.

Removes the GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersDeleteRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
  } satisfies GameServersDeleteRequest;

  try {
    const data = await api.gameServersDelete(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |

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
| **204** | GameServer resource deleted |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersGet

> GameServerGameServerRead gameServersGet(id)

Retrieves a GameServer resource.

Retrieves a GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersGetRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
  } satisfies GameServersGetRequest;

  try {
    const data = await api.gameServersGet(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer resource |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersList

> Array&lt;GameServerGameServerRead&gt; gameServersList(page)

Retrieves the collection of GameServer resources.

Retrieves the collection of GameServer resources.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersListRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // number | The collection page number (optional)
    page: 56,
  } satisfies GameServersListRequest;

  try {
    const data = await api.gameServersList(body);
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

[**Array&lt;GameServerGameServerRead&gt;**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer collection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersRestart

> GameServerGameServerRead gameServersRestart(id)

Creates a GameServer resource.

Creates a GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersRestartRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
  } satisfies GameServersRestartRequest;

  try {
    const data = await api.gameServersRestart(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersStart

> GameServerGameServerRead gameServersStart(id)

Creates a GameServer resource.

Creates a GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersStartRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
  } satisfies GameServersStartRequest;

  try {
    const data = await api.gameServersStart(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersStop

> GameServerGameServerRead gameServersStop(id)

Creates a GameServer resource.

Creates a GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersStopRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
  } satisfies GameServersStopRequest;

  try {
    const data = await api.gameServersStop(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer resource created |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gameServersUpdate

> GameServerGameServerRead gameServersUpdate(id, gameServerGameServerSettingsInputJsonMergePatch)

Updates the GameServer resource.

Updates the GameServer resource.

### Example

```ts
import {
  Configuration,
  GameServerApi,
} from '@someones-computer/sdk-js';
import type { GameServersUpdateRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GameServerApi(config);

  const body = {
    // string | GameServer identifier
    id: id_example,
    // GameServerGameServerSettingsInputJsonMergePatch | The updated GameServer resource
    gameServerGameServerSettingsInputJsonMergePatch: ...,
  } satisfies GameServersUpdateRequest;

  try {
    const data = await api.gameServersUpdate(body);
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
| **id** | `string` | GameServer identifier | [Defaults to `undefined`] |
| **gameServerGameServerSettingsInputJsonMergePatch** | [GameServerGameServerSettingsInputJsonMergePatch](GameServerGameServerSettingsInputJsonMergePatch.md) | The updated GameServer resource | |

### Return type

[**GameServerGameServerRead**](GameServerGameServerRead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/merge-patch+json`
- **Accept**: `application/json`, `application/problem+json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GameServer resource updated |  -  |
| **400** | Invalid input |  -  |
| **422** | An error occurred |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

