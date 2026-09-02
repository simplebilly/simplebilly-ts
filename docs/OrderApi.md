# OrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addOrderTags**](OrderApi.md#addordertags) | **POST** /api/v1/orders/{order_id}/tags |  |
| [**findOrderByExternalRef**](OrderApi.md#findorderbyexternalref) | **GET** /api/v1/orders/by-ext-ref/{ext_ref} |  |
| [**getOrder**](OrderApi.md#getorder) | **GET** /api/v1/order/{order_number} |  |
| [**getOrders**](OrderApi.md#getorders) | **GET** /api/v1/orders |  |
| [**patchOrder**](OrderApi.md#patchorder) | **PATCH** /api/v1/orders/{order_id} |  |
| [**replaceOrderTags**](OrderApi.md#replaceordertags) | **PUT** /api/v1/orders/{order_id}/tags |  |
| [**updateOrderState**](OrderApi.md#updateorderstate) | **PUT** /api/v1/orders/{order_id}/state |  |



## addOrderTags

> Order addOrderTags(orderId, orderTagsRequest)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { AddOrderTagsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    orderId: orderId_example,
    // OrderTagsRequest
    orderTagsRequest: ...,
  } satisfies AddOrderTagsRequest;

  try {
    const data = await api.addOrderTags(body);
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
| **orderId** | `string` |  | [Defaults to `undefined`] |
| **orderTagsRequest** | [OrderTagsRequest](OrderTagsRequest.md) |  | |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tags added |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## findOrderByExternalRef

> Order findOrderByExternalRef(extRef)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { FindOrderByExternalRefRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    extRef: extRef_example,
  } satisfies FindOrderByExternalRefRequest;

  try {
    const data = await api.findOrderByExternalRef(body);
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
| **extRef** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order found |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrder

> Order getOrder(orderNumber)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { GetOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
  } satisfies GetOrderRequest;

  try {
    const data = await api.getOrder(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order found |  -  |
| **400** | Bad Request |  -  |
| **404** | Order not found |  -  |
| **500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrders

> Array&lt;Order&gt; getOrders(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { GetOrdersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetOrdersRequest;

  try {
    const data = await api.getOrders(body);
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
| **includeDeleted** | `boolean` | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Order&gt;**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Orders found |  -  |
| **400** | Bad Request |  -  |
| **404** | No orders found |  -  |
| **500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## patchOrder

> Order patchOrder(orderId, body)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { PatchOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    orderId: orderId_example,
    // any
    body: ...,
  } satisfies PatchOrderRequest;

  try {
    const data = await api.patchOrder(body);
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
| **orderId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order updated |  -  |
| **400** | Bad request |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## replaceOrderTags

> Order replaceOrderTags(orderId, orderTagsRequest)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { ReplaceOrderTagsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    orderId: orderId_example,
    // OrderTagsRequest
    orderTagsRequest: ...,
  } satisfies ReplaceOrderTagsRequest;

  try {
    const data = await api.replaceOrderTags(body);
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
| **orderId** | `string` |  | [Defaults to `undefined`] |
| **orderTagsRequest** | [OrderTagsRequest](OrderTagsRequest.md) |  | |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tags replaced |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateOrderState

> Order updateOrderState(orderId, orderStateUpdate)



### Example

```ts
import {
  Configuration,
  OrderApi,
} from '@simplebilly/api';
import type { UpdateOrderStateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderApi(config);

  const body = {
    // string
    orderId: orderId_example,
    // OrderStateUpdate
    orderStateUpdate: ...,
  } satisfies UpdateOrderStateRequest;

  try {
    const data = await api.updateOrderState(body);
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
| **orderId** | `string` |  | [Defaults to `undefined`] |
| **orderStateUpdate** | [OrderStateUpdate](OrderStateUpdate.md) |  | |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order state updated |  -  |
| **400** | Bad request |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

