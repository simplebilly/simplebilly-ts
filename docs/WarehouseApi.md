# WarehouseApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createWarehouse**](WarehouseApi.md#createwarehouse) | **POST** /api/v1/warehouses |  |
| [**deleteWarehouse**](WarehouseApi.md#deletewarehouse) | **DELETE** /api/v1/warehouses/{warehouse_id} |  |
| [**getWarehouse**](WarehouseApi.md#getwarehouse) | **GET** /api/v1/warehouses/{warehouse_id} |  |
| [**listWarehouses**](WarehouseApi.md#listwarehouses) | **GET** /api/v1/warehouses/ |  |
| [**updateWarehouse**](WarehouseApi.md#updatewarehouse) | **PUT** /api/v1/warehouses/{warehouse_id} |  |



## createWarehouse

> Warehouse createWarehouse(warehouse)



### Example

```ts
import {
  Configuration,
  WarehouseApi,
} from '@simplebilly/api';
import type { CreateWarehouseRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseApi(config);

  const body = {
    // Warehouse
    warehouse: ...,
  } satisfies CreateWarehouseRequest;

  try {
    const data = await api.createWarehouse(body);
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
| **warehouse** | [Warehouse](Warehouse.md) |  | |

### Return type

[**Warehouse**](Warehouse.md)

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


## deleteWarehouse

> deleteWarehouse(warehouseId)



### Example

```ts
import {
  Configuration,
  WarehouseApi,
} from '@simplebilly/api';
import type { DeleteWarehouseRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
  } satisfies DeleteWarehouseRequest;

  try {
    const data = await api.deleteWarehouse(body);
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
| **warehouseId** | `string` |  | [Defaults to `undefined`] |

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
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getWarehouse

> Warehouse getWarehouse(warehouseId)



### Example

```ts
import {
  Configuration,
  WarehouseApi,
} from '@simplebilly/api';
import type { GetWarehouseRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
  } satisfies GetWarehouseRequest;

  try {
    const data = await api.getWarehouse(body);
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
| **warehouseId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Warehouse**](Warehouse.md)

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


## listWarehouses

> Array&lt;Warehouse&gt; listWarehouses(page, pageSize, search, isActive)



### Example

```ts
import {
  Configuration,
  WarehouseApi,
} from '@simplebilly/api';
import type { ListWarehousesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean (optional)
    isActive: true,
  } satisfies ListWarehousesRequest;

  try {
    const data = await api.listWarehouses(body);
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
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **isActive** | `boolean` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Warehouse&gt;**](Warehouse.md)

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


## updateWarehouse

> Warehouse updateWarehouse(warehouseId, body)



### Example

```ts
import {
  Configuration,
  WarehouseApi,
} from '@simplebilly/api';
import type { UpdateWarehouseRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
    // any
    body: ...,
  } satisfies UpdateWarehouseRequest;

  try {
    const data = await api.updateWarehouse(body);
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
| **warehouseId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**Warehouse**](Warehouse.md)

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

