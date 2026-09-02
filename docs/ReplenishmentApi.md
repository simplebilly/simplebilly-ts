# ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**applyReplenishments**](ReplenishmentApi.md#applyreplenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair. |
| [**getReplenishments**](ReplenishmentApi.md#getreplenishments) | **GET** /api/v1/replenishments |  |



## applyReplenishments

> any applyReplenishments(targetWarehouseId, sourceWarehouseId)

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

### Example

```ts
import {
  Configuration,
  ReplenishmentApi,
} from '@simplebilly/api';
import type { ApplyReplenishmentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReplenishmentApi(config);

  const body = {
    // string | Warehouse to be replenished. Defaults to the tenant\'s default warehouse. (optional)
    targetWarehouseId: targetWarehouseId_example,
    // string | Restrict source warehouses to this id. (optional)
    sourceWarehouseId: sourceWarehouseId_example,
  } satisfies ApplyReplenishmentsRequest;

  try {
    const data = await api.applyReplenishments(body);
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
| **targetWarehouseId** | `string` | Warehouse to be replenished. Defaults to the tenant\&#39;s default warehouse. | [Optional] [Defaults to `undefined`] |
| **sourceWarehouseId** | `string` | Restrict source warehouses to this id. | [Optional] [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReplenishments

> ReplenishmentResponse getReplenishments(targetWarehouseId, sourceWarehouseId)



### Example

```ts
import {
  Configuration,
  ReplenishmentApi,
} from '@simplebilly/api';
import type { GetReplenishmentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReplenishmentApi(config);

  const body = {
    // string | Warehouse to be replenished. Defaults to the tenant\'s default warehouse. (optional)
    targetWarehouseId: targetWarehouseId_example,
    // string | Restrict source warehouses to this id. (optional)
    sourceWarehouseId: sourceWarehouseId_example,
  } satisfies GetReplenishmentsRequest;

  try {
    const data = await api.getReplenishments(body);
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
| **targetWarehouseId** | `string` | Warehouse to be replenished. Defaults to the tenant\&#39;s default warehouse. | [Optional] [Defaults to `undefined`] |
| **sourceWarehouseId** | `string` | Restrict source warehouses to this id. | [Optional] [Defaults to `undefined`] |

### Return type

[**ReplenishmentResponse**](ReplenishmentResponse.md)

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

