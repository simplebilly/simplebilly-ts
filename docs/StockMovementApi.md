# StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getStockMovement**](StockMovementApi.md#getstockmovement) | **GET** /api/v1/stock-movements/{movement_id} |  |
| [**listStockMovements**](StockMovementApi.md#liststockmovements) | **GET** /api/v1/stock-movements/ |  |



## getStockMovement

> StockMovement getStockMovement(movementId)



### Example

```ts
import {
  Configuration,
  StockMovementApi,
} from '@simplebilly/api';
import type { GetStockMovementRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockMovementApi(config);

  const body = {
    // string
    movementId: movementId_example,
  } satisfies GetStockMovementRequest;

  try {
    const data = await api.getStockMovement(body);
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
| **movementId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**StockMovement**](StockMovement.md)

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


## listStockMovements

> Array&lt;StockMovement&gt; listStockMovements(page, pageSize, productId, warehouseId, movementType, from, to)



### Example

```ts
import {
  Configuration,
  StockMovementApi,
} from '@simplebilly/api';
import type { ListStockMovementsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StockMovementApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    warehouseId: warehouseId_example,
    // string (optional)
    movementType: movementType_example,
    // Date | Only movements on or after this date (inclusive). (optional)
    from: 2013-10-20,
    // Date | Only movements on or before this date (inclusive). (optional)
    to: 2013-10-20,
  } satisfies ListStockMovementsRequest;

  try {
    const data = await api.listStockMovements(body);
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
| **productId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **warehouseId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **movementType** | `string` |  | [Optional] [Defaults to `undefined`] |
| **from** | `Date` | Only movements on or after this date (inclusive). | [Optional] [Defaults to `undefined`] |
| **to** | `Date` | Only movements on or before this date (inclusive). | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;StockMovement&gt;**](StockMovement.md)

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

