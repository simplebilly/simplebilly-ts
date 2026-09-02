# ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createReturnOrder**](ReturnOrderApi.md#createreturnorder) | **POST** /api/v1/returns |  |
| [**deleteReturnOrder**](ReturnOrderApi.md#deletereturnorder) | **DELETE** /api/v1/returns/{return_order_id} |  |
| [**getReturnOrder**](ReturnOrderApi.md#getreturnorder) | **GET** /api/v1/returns/{return_order_id} |  |
| [**listReturnOrders**](ReturnOrderApi.md#listreturnorders) | **GET** /api/v1/returns/ |  |
| [**returnLogisticsQueue**](ReturnOrderApi.md#returnlogisticsqueue) | **GET** /api/v1/returns/logistics-queue |  |
| [**returnLogisticsSummary**](ReturnOrderApi.md#returnlogisticssummary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse. |
| [**updateReturnOrder**](ReturnOrderApi.md#updatereturnorder) | **PUT** /api/v1/returns/{return_order_id} |  |
| [**updateReturnOrderStatus**](ReturnOrderApi.md#updatereturnorderstatus) | **PUT** /api/v1/returns/{return_order_id}/status |  |



## createReturnOrder

> ReturnOrder createReturnOrder(returnOrder)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { CreateReturnOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // ReturnOrder
    returnOrder: ...,
  } satisfies CreateReturnOrderRequest;

  try {
    const data = await api.createReturnOrder(body);
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
| **returnOrder** | [ReturnOrder](ReturnOrder.md) |  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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


## deleteReturnOrder

> deleteReturnOrder(returnOrderId)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { DeleteReturnOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // string
    returnOrderId: returnOrderId_example,
  } satisfies DeleteReturnOrderRequest;

  try {
    const data = await api.deleteReturnOrder(body);
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
| **returnOrderId** | `string` |  | [Defaults to `undefined`] |

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


## getReturnOrder

> ReturnOrder getReturnOrder(returnOrderId)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { GetReturnOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // string
    returnOrderId: returnOrderId_example,
  } satisfies GetReturnOrderRequest;

  try {
    const data = await api.getReturnOrder(body);
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
| **returnOrderId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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


## listReturnOrders

> Array&lt;ReturnOrder&gt; listReturnOrders(page, pageSize, status, customerName, orderNumber)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { ListReturnOrdersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    customerName: customerName_example,
    // string (optional)
    orderNumber: orderNumber_example,
  } satisfies ListReturnOrdersRequest;

  try {
    const data = await api.listReturnOrders(body);
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
| **customerName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **orderNumber** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ReturnOrder&gt;**](ReturnOrder.md)

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


## returnLogisticsQueue

> Array&lt;ReturnLogisticsQueueItem&gt; returnLogisticsQueue()



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { ReturnLogisticsQueueRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  try {
    const data = await api.returnLogisticsQueue();
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

[**Array&lt;ReturnLogisticsQueueItem&gt;**](ReturnLogisticsQueueItem.md)

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


## returnLogisticsSummary

> ReturnLogisticsSummary returnLogisticsSummary()

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { ReturnLogisticsSummaryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  try {
    const data = await api.returnLogisticsSummary();
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

[**ReturnLogisticsSummary**](ReturnLogisticsSummary.md)

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


## updateReturnOrder

> ReturnOrder updateReturnOrder(returnOrderId, body)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { UpdateReturnOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // string
    returnOrderId: returnOrderId_example,
    // any
    body: ...,
  } satisfies UpdateReturnOrderRequest;

  try {
    const data = await api.updateReturnOrder(body);
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
| **returnOrderId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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


## updateReturnOrderStatus

> ReturnOrder updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate)



### Example

```ts
import {
  Configuration,
  ReturnOrderApi,
} from '@simplebilly/api';
import type { UpdateReturnOrderStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReturnOrderApi(config);

  const body = {
    // string
    returnOrderId: returnOrderId_example,
    // ReturnOrderStatusUpdate
    returnOrderStatusUpdate: ...,
  } satisfies UpdateReturnOrderStatusRequest;

  try {
    const data = await api.updateReturnOrderStatus(body);
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
| **returnOrderId** | `string` |  | [Defaults to `undefined`] |
| **returnOrderStatusUpdate** | [ReturnOrderStatusUpdate](ReturnOrderStatusUpdate.md) |  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

