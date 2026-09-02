# InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createInventoryCount**](InventoryCountApi.md#createinventorycount) | **POST** /api/v1/inventory-counts |  |
| [**deleteInventoryCount**](InventoryCountApi.md#deleteinventorycount) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**generateInventoryCount**](InventoryCountApi.md#generateinventorycount) | **POST** /api/v1/inventory-counts/generate |  |
| [**getInventoryCount**](InventoryCountApi.md#getinventorycount) | **GET** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**listInventoryCounts**](InventoryCountApi.md#listinventorycounts) | **GET** /api/v1/inventory-counts/ |  |
| [**updateInventoryCount**](InventoryCountApi.md#updateinventorycount) | **PUT** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**updateInventoryCountStatus**](InventoryCountApi.md#updateinventorycountstatus) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status |  |



## createInventoryCount

> InventoryCount createInventoryCount(inventoryCount)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { CreateInventoryCountRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // InventoryCount
    inventoryCount: ...,
  } satisfies CreateInventoryCountRequest;

  try {
    const data = await api.createInventoryCount(body);
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
| **inventoryCount** | [InventoryCount](InventoryCount.md) |  | |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteInventoryCount

> deleteInventoryCount(inventoryCountId)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { DeleteInventoryCountRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // string
    inventoryCountId: inventoryCountId_example,
  } satisfies DeleteInventoryCountRequest;

  try {
    const data = await api.deleteInventoryCount(body);
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
| **inventoryCountId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | No Content |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## generateInventoryCount

> InventoryCount generateInventoryCount(generateCountRequest)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { GenerateInventoryCountRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // GenerateCountRequest
    generateCountRequest: ...,
  } satisfies GenerateInventoryCountRequest;

  try {
    const data = await api.generateInventoryCount(body);
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
| **generateCountRequest** | [GenerateCountRequest](GenerateCountRequest.md) |  | |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInventoryCount

> InventoryCount getInventoryCount(inventoryCountId)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { GetInventoryCountRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // string
    inventoryCountId: inventoryCountId_example,
  } satisfies GetInventoryCountRequest;

  try {
    const data = await api.getInventoryCount(body);
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
| **inventoryCountId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listInventoryCounts

> Array&lt;InventoryCount&gt; listInventoryCounts(page, pageSize, status, warehouseId)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { ListInventoryCountsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    warehouseId: warehouseId_example,
  } satisfies ListInventoryCountsRequest;

  try {
    const data = await api.listInventoryCounts(body);
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
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **warehouseId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;InventoryCount&gt;**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateInventoryCount

> InventoryCount updateInventoryCount(inventoryCountId, body)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { UpdateInventoryCountRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // string
    inventoryCountId: inventoryCountId_example,
    // any
    body: ...,
  } satisfies UpdateInventoryCountRequest;

  try {
    const data = await api.updateInventoryCount(body);
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
| **inventoryCountId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateInventoryCountStatus

> InventoryCount updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate)



### Example

```ts
import {
  Configuration,
  InventoryCountApi,
} from '@simplebilly/api';
import type { UpdateInventoryCountStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InventoryCountApi(config);

  const body = {
    // string
    inventoryCountId: inventoryCountId_example,
    // InventoryCountStatusUpdate
    inventoryCountStatusUpdate: ...,
  } satisfies UpdateInventoryCountStatusRequest;

  try {
    const data = await api.updateInventoryCountStatus(body);
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
| **inventoryCountId** | `string` |  | [Defaults to `undefined`] |
| **inventoryCountStatusUpdate** | [InventoryCountStatusUpdate](InventoryCountStatusUpdate.md) |  | |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

