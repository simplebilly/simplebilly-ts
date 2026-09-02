# StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createStockTransfer**](StockTransferApi.md#createstocktransfer) | **POST** /api/v1/stock-transfers |  |
| [**deleteStockTransfer**](StockTransferApi.md#deletestocktransfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} |  |
| [**getStockTransfer**](StockTransferApi.md#getstocktransfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} |  |
| [**listStockTransfers**](StockTransferApi.md#liststocktransfers) | **GET** /api/v1/stock-transfers/ |  |
| [**updateStockTransferStatus**](StockTransferApi.md#updatestocktransferstatus) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status |  |



## createStockTransfer

> StockTransfer createStockTransfer(stockTransfer)



### Example

```ts
import {
  Configuration,
  StockTransferApi,
} from '@simplebilly/api';
import type { CreateStockTransferRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockTransferApi(config);

  const body = {
    // StockTransfer
    stockTransfer: ...,
  } satisfies CreateStockTransferRequest;

  try {
    const data = await api.createStockTransfer(body);
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
| **stockTransfer** | [StockTransfer](StockTransfer.md) |  | |

### Return type

[**StockTransfer**](StockTransfer.md)

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


## deleteStockTransfer

> deleteStockTransfer(stockTransferId)



### Example

```ts
import {
  Configuration,
  StockTransferApi,
} from '@simplebilly/api';
import type { DeleteStockTransferRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockTransferApi(config);

  const body = {
    // string
    stockTransferId: stockTransferId_example,
  } satisfies DeleteStockTransferRequest;

  try {
    const data = await api.deleteStockTransfer(body);
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
| **stockTransferId** | `string` |  | [Defaults to `undefined`] |

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


## getStockTransfer

> StockTransfer getStockTransfer(stockTransferId)



### Example

```ts
import {
  Configuration,
  StockTransferApi,
} from '@simplebilly/api';
import type { GetStockTransferRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockTransferApi(config);

  const body = {
    // string
    stockTransferId: stockTransferId_example,
  } satisfies GetStockTransferRequest;

  try {
    const data = await api.getStockTransfer(body);
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
| **stockTransferId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**StockTransfer**](StockTransfer.md)

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


## listStockTransfers

> Array&lt;StockTransfer&gt; listStockTransfers(page, pageSize, status, warehouseId)



### Example

```ts
import {
  Configuration,
  StockTransferApi,
} from '@simplebilly/api';
import type { ListStockTransfersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockTransferApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    warehouseId: warehouseId_example,
  } satisfies ListStockTransfersRequest;

  try {
    const data = await api.listStockTransfers(body);
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

[**Array&lt;StockTransfer&gt;**](StockTransfer.md)

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


## updateStockTransferStatus

> StockTransfer updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate)



### Example

```ts
import {
  Configuration,
  StockTransferApi,
} from '@simplebilly/api';
import type { UpdateStockTransferStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockTransferApi(config);

  const body = {
    // string
    stockTransferId: stockTransferId_example,
    // StockTransferStatusUpdate
    stockTransferStatusUpdate: ...,
  } satisfies UpdateStockTransferStatusRequest;

  try {
    const data = await api.updateStockTransferStatus(body);
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
| **stockTransferId** | `string` |  | [Defaults to `undefined`] |
| **stockTransferStatusUpdate** | [StockTransferStatusUpdate](StockTransferStatusUpdate.md) |  | |

### Return type

[**StockTransfer**](StockTransfer.md)

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

