# ProductionOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProductionOrder**](ProductionOrderApi.md#createproductionorder) | **POST** /api/v1/production-orders |  |
| [**deleteProductionOrder**](ProductionOrderApi.md#deleteproductionorder) | **DELETE** /api/v1/production-orders/{production_order_id} |  |
| [**getProductionOrder**](ProductionOrderApi.md#getproductionorder) | **GET** /api/v1/production-orders/{production_order_id} |  |
| [**listProductionOrders**](ProductionOrderApi.md#listproductionorders) | **GET** /api/v1/production-orders/ |  |
| [**productionOrderCosting**](ProductionOrderApi.md#productionordercosting) | **GET** /api/v1/production-orders/{production_order_id}/costing | Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product\&#39;s sale price. |
| [**updateProductionOrder**](ProductionOrderApi.md#updateproductionorder) | **PUT** /api/v1/production-orders/{production_order_id} |  |
| [**updateProductionOrderStatus**](ProductionOrderApi.md#updateproductionorderstatus) | **PUT** /api/v1/production-orders/{production_order_id}/status |  |



## createProductionOrder

> ProductionOrder createProductionOrder(productionOrder)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { CreateProductionOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // ProductionOrder
    productionOrder: ...,
  } satisfies CreateProductionOrderRequest;

  try {
    const data = await api.createProductionOrder(body);
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
| **productionOrder** | [ProductionOrder](ProductionOrder.md) |  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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


## deleteProductionOrder

> deleteProductionOrder(productionOrderId)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { DeleteProductionOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // string
    productionOrderId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteProductionOrderRequest;

  try {
    const data = await api.deleteProductionOrder(body);
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
| **productionOrderId** | `string` |  | [Defaults to `undefined`] |

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
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProductionOrder

> ProductionOrder getProductionOrder(productionOrderId)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { GetProductionOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // string
    productionOrderId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetProductionOrderRequest;

  try {
    const data = await api.getProductionOrder(body);
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
| **productionOrderId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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


## listProductionOrders

> Array&lt;ProductionOrder&gt; listProductionOrders(page, pageSize, search, status)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { ListProductionOrdersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // string | Filter by status. (optional)
    status: status_example,
  } satisfies ListProductionOrdersRequest;

  try {
    const data = await api.listProductionOrders(body);
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
| **status** | `string` | Filter by status. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProductionOrder&gt;**](ProductionOrder.md)

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


## productionOrderCosting

> ProductionOrderCosting productionOrderCosting(productionOrderId)

Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product\&#39;s sale price.

### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { ProductionOrderCostingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // string
    productionOrderId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ProductionOrderCostingRequest;

  try {
    const data = await api.productionOrderCosting(body);
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
| **productionOrderId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProductionOrderCosting**](ProductionOrderCosting.md)

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


## updateProductionOrder

> ProductionOrder updateProductionOrder(productionOrderId, productionOrder)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { UpdateProductionOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // string
    productionOrderId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ProductionOrder
    productionOrder: ...,
  } satisfies UpdateProductionOrderRequest;

  try {
    const data = await api.updateProductionOrder(body);
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
| **productionOrderId** | `string` |  | [Defaults to `undefined`] |
| **productionOrder** | [ProductionOrder](ProductionOrder.md) |  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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


## updateProductionOrderStatus

> ProductionOrder updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate)



### Example

```ts
import {
  Configuration,
  ProductionOrderApi,
} from '@simplebilly/api';
import type { UpdateProductionOrderStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductionOrderApi(config);

  const body = {
    // string
    productionOrderId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ProductionOrderStatusUpdate
    productionOrderStatusUpdate: ...,
  } satisfies UpdateProductionOrderStatusRequest;

  try {
    const data = await api.updateProductionOrderStatus(body);
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
| **productionOrderId** | `string` |  | [Defaults to `undefined`] |
| **productionOrderStatusUpdate** | [ProductionOrderStatusUpdate](ProductionOrderStatusUpdate.md) |  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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

