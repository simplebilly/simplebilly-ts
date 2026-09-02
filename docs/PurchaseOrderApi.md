# PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPurchaseOrder**](PurchaseOrderApi.md#createpurchaseorder) | **POST** /api/v1/purchase-orders |  |
| [**deletePurchaseOrder**](PurchaseOrderApi.md#deletepurchaseorder) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**getPurchaseOrder**](PurchaseOrderApi.md#getpurchaseorder) | **GET** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**listPurchaseOrders**](PurchaseOrderApi.md#listpurchaseorders) | **GET** /api/v1/purchase-orders/ |  |
| [**matchInvoice**](PurchaseOrderApi.md#matchinvoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product. |
| [**updatePurchaseOrder**](PurchaseOrderApi.md#updatepurchaseorder) | **PUT** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**updatePurchaseOrderStatus**](PurchaseOrderApi.md#updatepurchaseorderstatus) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status |  |



## createPurchaseOrder

> PurchaseOrder createPurchaseOrder(purchaseOrder)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { CreatePurchaseOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // PurchaseOrder
    purchaseOrder: ...,
  } satisfies CreatePurchaseOrderRequest;

  try {
    const data = await api.createPurchaseOrder(body);
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
| **purchaseOrder** | [PurchaseOrder](PurchaseOrder.md) |  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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


## deletePurchaseOrder

> deletePurchaseOrder(purchaseOrderId)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { DeletePurchaseOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // string
    purchaseOrderId: purchaseOrderId_example,
  } satisfies DeletePurchaseOrderRequest;

  try {
    const data = await api.deletePurchaseOrder(body);
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
| **purchaseOrderId** | `string` |  | [Defaults to `undefined`] |

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


## getPurchaseOrder

> PurchaseOrder getPurchaseOrder(purchaseOrderId)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { GetPurchaseOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // string
    purchaseOrderId: purchaseOrderId_example,
  } satisfies GetPurchaseOrderRequest;

  try {
    const data = await api.getPurchaseOrder(body);
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
| **purchaseOrderId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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


## listPurchaseOrders

> Array&lt;PurchaseOrder&gt; listPurchaseOrders(page, pageSize, status, supplierName, search)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { ListPurchaseOrdersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    supplierName: supplierName_example,
    // string (optional)
    search: search_example,
  } satisfies ListPurchaseOrdersRequest;

  try {
    const data = await api.listPurchaseOrders(body);
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
| **supplierName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;PurchaseOrder&gt;**](PurchaseOrder.md)

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


## matchInvoice

> any matchInvoice(purchaseOrderId, invoiceMatchRequest)

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { MatchInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // string
    purchaseOrderId: purchaseOrderId_example,
    // InvoiceMatchRequest
    invoiceMatchRequest: ...,
  } satisfies MatchInvoiceRequest;

  try {
    const data = await api.matchInvoice(body);
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
| **purchaseOrderId** | `string` |  | [Defaults to `undefined`] |
| **invoiceMatchRequest** | [InvoiceMatchRequest](InvoiceMatchRequest.md) |  | |

### Return type

**any**

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


## updatePurchaseOrder

> PurchaseOrder updatePurchaseOrder(purchaseOrderId, body)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { UpdatePurchaseOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // string
    purchaseOrderId: purchaseOrderId_example,
    // any
    body: ...,
  } satisfies UpdatePurchaseOrderRequest;

  try {
    const data = await api.updatePurchaseOrder(body);
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
| **purchaseOrderId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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


## updatePurchaseOrderStatus

> PurchaseOrder updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate)



### Example

```ts
import {
  Configuration,
  PurchaseOrderApi,
} from '@simplebilly/api';
import type { UpdatePurchaseOrderStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchaseOrderApi(config);

  const body = {
    // string
    purchaseOrderId: purchaseOrderId_example,
    // PurchaseOrderStatusUpdate
    purchaseOrderStatusUpdate: ...,
  } satisfies UpdatePurchaseOrderStatusRequest;

  try {
    const data = await api.updatePurchaseOrderStatus(body);
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
| **purchaseOrderId** | `string` |  | [Defaults to `undefined`] |
| **purchaseOrderStatusUpdate** | [PurchaseOrderStatusUpdate](PurchaseOrderStatusUpdate.md) |  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

