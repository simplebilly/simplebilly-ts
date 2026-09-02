# MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createConnectionApi**](MarketplaceApiApi.md#createconnectionapi) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms) |
| [**deleteConnectionApi**](MarketplaceApiApi.md#deleteconnectionapi) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection |
| [**getConnectionApi**](MarketplaceApiApi.md#getconnectionapi) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection |
| [**getSyncDirectionApi**](MarketplaceApiApi.md#getsyncdirectionapi) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection |
| [**getSyncLogsApi**](MarketplaceApiApi.md#getsynclogsapi) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection |
| [**listConnectionsApi**](MarketplaceApiApi.md#listconnectionsapi) | **GET** /api/v1/marketplace/connections | List connections for the current tenant |
| [**listPlatformsApi**](MarketplaceApiApi.md#listplatformsapi) | **GET** /api/v1/marketplace/platforms | List all supported platforms |
| [**oauthAuthorizeApi**](MarketplaceApiApi.md#oauthauthorizeapi) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow |
| [**oauthCallbackApi**](MarketplaceApiApi.md#oauthcallbackapi) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization |
| [**triggerSyncApi**](MarketplaceApiApi.md#triggersyncapi) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection |
| [**updateConnectionApi**](MarketplaceApiApi.md#updateconnectionapi) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection |
| [**updateSyncDirectionApi**](MarketplaceApiApi.md#updatesyncdirectionapi) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection |
| [**webhookReceiverApi**](MarketplaceApiApi.md#webhookreceiverapi) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver |



## createConnectionApi

> MarketplaceConnection createConnectionApi(createConnectionRequest)

Create a new connection (for API-key based platforms)

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { CreateConnectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // CreateConnectionRequest
    createConnectionRequest: ...,
  } satisfies CreateConnectionApiRequest;

  try {
    const data = await api.createConnectionApi(body);
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
| **createConnectionRequest** | [CreateConnectionRequest](CreateConnectionRequest.md) |  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteConnectionApi

> deleteConnectionApi(connectionId)

Soft-delete a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { DeleteConnectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
  } satisfies DeleteConnectionApiRequest;

  try {
    const data = await api.deleteConnectionApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getConnectionApi

> MarketplaceConnection getConnectionApi(connectionId)

Get a single connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { GetConnectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
  } satisfies GetConnectionApiRequest;

  try {
    const data = await api.getConnectionApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSyncDirectionApi

> getSyncDirectionApi(connectionId)

Get current sync direction configuration for a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { GetSyncDirectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
  } satisfies GetSyncDirectionApiRequest;

  try {
    const data = await api.getSyncDirectionApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current sync directions |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSyncLogsApi

> Array&lt;SyncLog&gt; getSyncLogsApi(connectionId)

Get sync logs for a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { GetSyncLogsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
  } satisfies GetSyncLogsApiRequest;

  try {
    const data = await api.getSyncLogsApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SyncLog&gt;**](SyncLog.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Sync logs |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listConnectionsApi

> Array&lt;MarketplaceConnection&gt; listConnectionsApi()

List connections for the current tenant

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { ListConnectionsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  try {
    const data = await api.listConnectionsApi();
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

[**Array&lt;MarketplaceConnection&gt;**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of connections |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPlatformsApi

> Array&lt;PlatformInfo&gt; listPlatformsApi()

List all supported platforms

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { ListPlatformsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  try {
    const data = await api.listPlatformsApi();
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

[**Array&lt;PlatformInfo&gt;**](PlatformInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Supported platforms |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## oauthAuthorizeApi

> OAuthAuthorizeResponse oauthAuthorizeApi(oAuthAuthorizeRequest)

OAuth: initiate authorization flow

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { OauthAuthorizeApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // OAuthAuthorizeRequest
    oAuthAuthorizeRequest: ...,
  } satisfies OauthAuthorizeApiRequest;

  try {
    const data = await api.oauthAuthorizeApi(body);
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
| **oAuthAuthorizeRequest** | [OAuthAuthorizeRequest](OAuthAuthorizeRequest.md) |  | |

### Return type

[**OAuthAuthorizeResponse**](OAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Authorization URL |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## oauthCallbackApi

> MarketplaceConnection oauthCallbackApi(oAuthCallbackRequest)

OAuth: handle callback after authorization

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { OauthCallbackApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // OAuthCallbackRequest
    oAuthCallbackRequest: ...,
  } satisfies OauthCallbackApiRequest;

  try {
    const data = await api.oauthCallbackApi(body);
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
| **oAuthCallbackRequest** | [OAuthCallbackRequest](OAuthCallbackRequest.md) |  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection created/updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## triggerSyncApi

> SyncSummary triggerSyncApi(connectionId, syncType, direction)

Trigger sync for a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { TriggerSyncApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
    // string (optional)
    syncType: syncType_example,
    // string (optional)
    direction: direction_example,
  } satisfies TriggerSyncApiRequest;

  try {
    const data = await api.triggerSyncApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |
| **syncType** | `string` |  | [Optional] [Defaults to `undefined`] |
| **direction** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**SyncSummary**](SyncSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Sync triggered |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateConnectionApi

> MarketplaceConnection updateConnectionApi(connectionId, updateConnectionRequest)

Update a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { UpdateConnectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
    // UpdateConnectionRequest
    updateConnectionRequest: ...,
  } satisfies UpdateConnectionApiRequest;

  try {
    const data = await api.updateConnectionApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |
| **updateConnectionRequest** | [UpdateConnectionRequest](UpdateConnectionRequest.md) |  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateSyncDirectionApi

> updateSyncDirectionApi(connectionId, updateSyncDirectionRequest)

Update per-entity sync direction configuration for a connection

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { UpdateSyncDirectionApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    connectionId: connectionId_example,
    // UpdateSyncDirectionRequest
    updateSyncDirectionRequest: ...,
  } satisfies UpdateSyncDirectionApiRequest;

  try {
    const data = await api.updateSyncDirectionApi(body);
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
| **connectionId** | `string` |  | [Defaults to `undefined`] |
| **updateSyncDirectionRequest** | [UpdateSyncDirectionRequest](UpdateSyncDirectionRequest.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Sync directions updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## webhookReceiverApi

> webhookReceiverApi(platform, connectionId)

Webhook receiver

### Example

```ts
import {
  Configuration,
  MarketplaceApiApi,
} from '@simplebilly/api';
import type { WebhookReceiverApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MarketplaceApiApi(config);

  const body = {
    // string
    platform: platform_example,
    // string
    connectionId: connectionId_example,
  } satisfies WebhookReceiverApiRequest;

  try {
    const data = await api.webhookReceiverApi(body);
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
| **platform** | `string` |  | [Defaults to `undefined`] |
| **connectionId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received |  -  |
| **401** | Invalid signature |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

