# ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**applyReorderProposal**](ReorderProposalApi.md#applyreorderproposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order. |
| [**getReorderProposal**](ReorderProposalApi.md#getreorderproposal) | **GET** /api/v1/reorder-proposals |  |



## applyReorderProposal

> any applyReorderProposal(configuredOnly, warehouseId)

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated with the current reorder quantity per product.

### Example

```ts
import {
  Configuration,
  ReorderProposalApi,
} from '@simplebilly/api';
import type { ApplyReorderProposalRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReorderProposalApi(config);

  const body = {
    // boolean | Only include products with a reorder point configured (`min_stock`). (optional)
    configuredOnly: true,
    // string | Limit to a single warehouse id. (optional)
    warehouseId: warehouseId_example,
  } satisfies ApplyReorderProposalRequest;

  try {
    const data = await api.applyReorderProposal(body);
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
| **configuredOnly** | `boolean` | Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [Optional] [Defaults to `undefined`] |
| **warehouseId** | `string` | Limit to a single warehouse id. | [Optional] [Defaults to `undefined`] |

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


## getReorderProposal

> ReorderProposalResponse getReorderProposal(configuredOnly, warehouseId)



### Example

```ts
import {
  Configuration,
  ReorderProposalApi,
} from '@simplebilly/api';
import type { GetReorderProposalRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReorderProposalApi(config);

  const body = {
    // boolean | Only include products with a reorder point configured (`min_stock`). (optional)
    configuredOnly: true,
    // string | Limit to a single warehouse id. (optional)
    warehouseId: warehouseId_example,
  } satisfies GetReorderProposalRequest;

  try {
    const data = await api.getReorderProposal(body);
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
| **configuredOnly** | `boolean` | Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [Optional] [Defaults to `undefined`] |
| **warehouseId** | `string` | Limit to a single warehouse id. | [Optional] [Defaults to `undefined`] |

### Return type

[**ReorderProposalResponse**](ReorderProposalResponse.md)

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

