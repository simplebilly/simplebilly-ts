# GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createGoodsReceipt**](GoodsReceiptApi.md#creategoodsreceipt) | **POST** /api/v1/goods-receipts |  |
| [**deleteGoodsReceipt**](GoodsReceiptApi.md#deletegoodsreceipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} |  |
| [**getGoodsReceipt**](GoodsReceiptApi.md#getgoodsreceipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} |  |
| [**listGoodsReceipts**](GoodsReceiptApi.md#listgoodsreceipts) | **GET** /api/v1/goods-receipts/ |  |



## createGoodsReceipt

> GoodsReceipt createGoodsReceipt(goodsReceipt)



### Example

```ts
import {
  Configuration,
  GoodsReceiptApi,
} from '@simplebilly/api';
import type { CreateGoodsReceiptRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GoodsReceiptApi(config);

  const body = {
    // GoodsReceipt
    goodsReceipt: ...,
  } satisfies CreateGoodsReceiptRequest;

  try {
    const data = await api.createGoodsReceipt(body);
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
| **goodsReceipt** | [GoodsReceipt](GoodsReceipt.md) |  | |

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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


## deleteGoodsReceipt

> deleteGoodsReceipt(goodsReceiptId)



### Example

```ts
import {
  Configuration,
  GoodsReceiptApi,
} from '@simplebilly/api';
import type { DeleteGoodsReceiptRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GoodsReceiptApi(config);

  const body = {
    // string
    goodsReceiptId: goodsReceiptId_example,
  } satisfies DeleteGoodsReceiptRequest;

  try {
    const data = await api.deleteGoodsReceipt(body);
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
| **goodsReceiptId** | `string` |  | [Defaults to `undefined`] |

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


## getGoodsReceipt

> GoodsReceipt getGoodsReceipt(goodsReceiptId)



### Example

```ts
import {
  Configuration,
  GoodsReceiptApi,
} from '@simplebilly/api';
import type { GetGoodsReceiptRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GoodsReceiptApi(config);

  const body = {
    // string
    goodsReceiptId: goodsReceiptId_example,
  } satisfies GetGoodsReceiptRequest;

  try {
    const data = await api.getGoodsReceipt(body);
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
| **goodsReceiptId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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


## listGoodsReceipts

> Array&lt;GoodsReceipt&gt; listGoodsReceipts(page, pageSize, purchaseOrderId, supplierName, warehouseId)



### Example

```ts
import {
  Configuration,
  GoodsReceiptApi,
} from '@simplebilly/api';
import type { ListGoodsReceiptsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GoodsReceiptApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    purchaseOrderId: purchaseOrderId_example,
    // string (optional)
    supplierName: supplierName_example,
    // string (optional)
    warehouseId: warehouseId_example,
  } satisfies ListGoodsReceiptsRequest;

  try {
    const data = await api.listGoodsReceipts(body);
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
| **purchaseOrderId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **warehouseId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;GoodsReceipt&gt;**](GoodsReceipt.md)

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

