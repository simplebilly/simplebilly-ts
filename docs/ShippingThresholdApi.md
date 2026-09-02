# ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createShippingThreshold**](ShippingThresholdApi.md#createshippingthreshold) | **POST** /api/v1/shipping-thresholds |  |
| [**deleteShippingThreshold**](ShippingThresholdApi.md#deleteshippingthreshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} |  |
| [**getDeliverable**](ShippingThresholdApi.md#getdeliverable) | **GET** /api/v1/shipping-thresholds/deliverable |  |
| [**getShippingThreshold**](ShippingThresholdApi.md#getshippingthreshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} |  |
| [**listShippingThresholds**](ShippingThresholdApi.md#listshippingthresholds) | **GET** /api/v1/shipping-thresholds/ |  |
| [**updateShippingThreshold**](ShippingThresholdApi.md#updateshippingthreshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} |  |



## createShippingThreshold

> ShippingThreshold createShippingThreshold(shippingThresholdCreate)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { CreateShippingThresholdRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // ShippingThresholdCreate
    shippingThresholdCreate: ...,
  } satisfies CreateShippingThresholdRequest;

  try {
    const data = await api.createShippingThreshold(body);
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
| **shippingThresholdCreate** | [ShippingThresholdCreate](ShippingThresholdCreate.md) |  | |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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


## deleteShippingThreshold

> deleteShippingThreshold(thresholdId)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { DeleteShippingThresholdRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // string
    thresholdId: thresholdId_example,
  } satisfies DeleteShippingThresholdRequest;

  try {
    const data = await api.deleteShippingThreshold(body);
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
| **thresholdId** | `string` |  | [Defaults to `undefined`] |

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


## getDeliverable

> DeliverableResponse getDeliverable(productId, warehouseId)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { GetDeliverableRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // string
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    warehouseId: warehouseId_example,
  } satisfies GetDeliverableRequest;

  try {
    const data = await api.getDeliverable(body);
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
| **warehouseId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**DeliverableResponse**](DeliverableResponse.md)

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


## getShippingThreshold

> ShippingThreshold getShippingThreshold(thresholdId)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { GetShippingThresholdRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // string
    thresholdId: thresholdId_example,
  } satisfies GetShippingThresholdRequest;

  try {
    const data = await api.getShippingThreshold(body);
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
| **thresholdId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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


## listShippingThresholds

> Array&lt;ShippingThreshold&gt; listShippingThresholds(page, pageSize, productId, warehouseId, isActive)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { ListShippingThresholdsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    warehouseId: warehouseId_example,
    // boolean (optional)
    isActive: true,
  } satisfies ListShippingThresholdsRequest;

  try {
    const data = await api.listShippingThresholds(body);
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
| **isActive** | `boolean` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ShippingThreshold&gt;**](ShippingThreshold.md)

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


## updateShippingThreshold

> ShippingThreshold updateShippingThreshold(thresholdId, shippingThresholdUpdate)



### Example

```ts
import {
  Configuration,
  ShippingThresholdApi,
} from '@simplebilly/api';
import type { UpdateShippingThresholdRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingThresholdApi(config);

  const body = {
    // string
    thresholdId: thresholdId_example,
    // ShippingThresholdUpdate
    shippingThresholdUpdate: ...,
  } satisfies UpdateShippingThresholdRequest;

  try {
    const data = await api.updateShippingThreshold(body);
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
| **thresholdId** | `string` |  | [Defaults to `undefined`] |
| **shippingThresholdUpdate** | [ShippingThresholdUpdate](ShippingThresholdUpdate.md) |  | |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

