# WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createWarehouseStock**](WarehouseStockApi.md#createwarehousestock) | **POST** /api/v1/warehouses/{warehouse_id}/stock |  |
| [**deleteWarehouseStock**](WarehouseStockApi.md#deletewarehousestock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} |  |
| [**listWarehouseStock**](WarehouseStockApi.md#listwarehousestock) | **GET** /api/v1/warehouses/{warehouse_id}/stock |  |
| [**updateWarehouseStock**](WarehouseStockApi.md#updatewarehousestock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} |  |



## createWarehouseStock

> WarehouseStock createWarehouseStock(warehouseId, stockAdjustment)



### Example

```ts
import {
  Configuration,
  WarehouseStockApi,
} from '@simplebilly/api';
import type { CreateWarehouseStockRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseStockApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
    // StockAdjustment
    stockAdjustment: ...,
  } satisfies CreateWarehouseStockRequest;

  try {
    const data = await api.createWarehouseStock(body);
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
| **stockAdjustment** | [StockAdjustment](StockAdjustment.md) |  | |

### Return type

[**WarehouseStock**](WarehouseStock.md)

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


## deleteWarehouseStock

> deleteWarehouseStock(warehouseId, productId)



### Example

```ts
import {
  Configuration,
  WarehouseStockApi,
} from '@simplebilly/api';
import type { DeleteWarehouseStockRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseStockApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
    // string
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteWarehouseStockRequest;

  try {
    const data = await api.deleteWarehouseStock(body);
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
| **productId** | `string` |  | [Defaults to `undefined`] |

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


## listWarehouseStock

> Array&lt;WarehouseStock&gt; listWarehouseStock(warehouseId)



### Example

```ts
import {
  Configuration,
  WarehouseStockApi,
} from '@simplebilly/api';
import type { ListWarehouseStockRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseStockApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
  } satisfies ListWarehouseStockRequest;

  try {
    const data = await api.listWarehouseStock(body);
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

[**Array&lt;WarehouseStock&gt;**](WarehouseStock.md)

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


## updateWarehouseStock

> WarehouseStock updateWarehouseStock(warehouseId, productId, stockAdjustment)



### Example

```ts
import {
  Configuration,
  WarehouseStockApi,
} from '@simplebilly/api';
import type { UpdateWarehouseStockRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WarehouseStockApi(config);

  const body = {
    // string
    warehouseId: warehouseId_example,
    // string
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // StockAdjustment
    stockAdjustment: ...,
  } satisfies UpdateWarehouseStockRequest;

  try {
    const data = await api.updateWarehouseStock(body);
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
| **productId** | `string` |  | [Defaults to `undefined`] |
| **stockAdjustment** | [StockAdjustment](StockAdjustment.md) |  | |

### Return type

[**WarehouseStock**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

