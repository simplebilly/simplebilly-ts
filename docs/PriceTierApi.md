# PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPriceTier**](PriceTierApi.md#createpricetier) | **POST** /api/v1/price-tiers |  |
| [**deletePriceTier**](PriceTierApi.md#deletepricetier) | **DELETE** /api/v1/price-tiers/{price_tier_id} |  |
| [**getPriceTier**](PriceTierApi.md#getpricetier) | **GET** /api/v1/price-tiers/{price_tier_id} |  |
| [**getResolvedPrice**](PriceTierApi.md#getresolvedprice) | **GET** /api/v1/price-tiers/resolved |  |
| [**listPriceTiers**](PriceTierApi.md#listpricetiers) | **GET** /api/v1/price-tiers/ |  |
| [**updatePriceTier**](PriceTierApi.md#updatepricetier) | **PUT** /api/v1/price-tiers/{price_tier_id} |  |



## createPriceTier

> PriceTier createPriceTier(priceTierCreate)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { CreatePriceTierRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // PriceTierCreate
    priceTierCreate: ...,
  } satisfies CreatePriceTierRequest;

  try {
    const data = await api.createPriceTier(body);
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
| **priceTierCreate** | [PriceTierCreate](PriceTierCreate.md) |  | |

### Return type

[**PriceTier**](PriceTier.md)

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


## deletePriceTier

> deletePriceTier(priceTierId)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { DeletePriceTierRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // string
    priceTierId: priceTierId_example,
  } satisfies DeletePriceTierRequest;

  try {
    const data = await api.deletePriceTier(body);
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
| **priceTierId** | `string` |  | [Defaults to `undefined`] |

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


## getPriceTier

> PriceTier getPriceTier(priceTierId)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { GetPriceTierRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // string
    priceTierId: priceTierId_example,
  } satisfies GetPriceTierRequest;

  try {
    const data = await api.getPriceTier(body);
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
| **priceTierId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PriceTier**](PriceTier.md)

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


## getResolvedPrice

> ResolvedPriceResponse getResolvedPrice(productId, quantity, contactId)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { GetResolvedPriceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // string
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // number (optional)
    quantity: 789,
    // string | Contact used to match customer-group-scoped tiers. (optional)
    contactId: contactId_example,
  } satisfies GetResolvedPriceRequest;

  try {
    const data = await api.getResolvedPrice(body);
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
| **productId** | `string` |  | [Defaults to `undefined`] |
| **quantity** | `number` |  | [Optional] [Defaults to `undefined`] |
| **contactId** | `string` | Contact used to match customer-group-scoped tiers. | [Optional] [Defaults to `undefined`] |

### Return type

[**ResolvedPriceResponse**](ResolvedPriceResponse.md)

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


## listPriceTiers

> Array&lt;PriceTier&gt; listPriceTiers(page, pageSize, productId, customerGroupId)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { ListPriceTiersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    customerGroupId: customerGroupId_example,
  } satisfies ListPriceTiersRequest;

  try {
    const data = await api.listPriceTiers(body);
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
| **customerGroupId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;PriceTier&gt;**](PriceTier.md)

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


## updatePriceTier

> PriceTier updatePriceTier(priceTierId, priceTierUpdate)



### Example

```ts
import {
  Configuration,
  PriceTierApi,
} from '@simplebilly/api';
import type { UpdatePriceTierRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PriceTierApi(config);

  const body = {
    // string
    priceTierId: priceTierId_example,
    // PriceTierUpdate
    priceTierUpdate: ...,
  } satisfies UpdatePriceTierRequest;

  try {
    const data = await api.updatePriceTier(body);
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
| **priceTierId** | `string` |  | [Defaults to `undefined`] |
| **priceTierUpdate** | [PriceTierUpdate](PriceTierUpdate.md) |  | |

### Return type

[**PriceTier**](PriceTier.md)

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

