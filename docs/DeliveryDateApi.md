# DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDeliveryDate**](DeliveryDateApi.md#createdeliverydate) | **POST** /api/v1/delivery-dates |  |
| [**deleteDeliveryDate**](DeliveryDateApi.md#deletedeliverydate) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**getDeliveryDate**](DeliveryDateApi.md#getdeliverydate) | **GET** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**getDeliveryPerformance**](DeliveryDateApi.md#getdeliveryperformance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period. |
| [**listDeliveryDates**](DeliveryDateApi.md#listdeliverydates) | **GET** /api/v1/delivery-dates/ |  |
| [**updateDeliveryDate**](DeliveryDateApi.md#updatedeliverydate) | **PUT** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**updateDeliveryDateStatus**](DeliveryDateApi.md#updatedeliverydatestatus) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status |  |



## createDeliveryDate

> DeliveryDate createDeliveryDate(deliveryDateCreate)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { CreateDeliveryDateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // DeliveryDateCreate
    deliveryDateCreate: ...,
  } satisfies CreateDeliveryDateRequest;

  try {
    const data = await api.createDeliveryDate(body);
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
| **deliveryDateCreate** | [DeliveryDateCreate](DeliveryDateCreate.md) |  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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


## deleteDeliveryDate

> deleteDeliveryDate(deliveryDateId)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { DeleteDeliveryDateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // string
    deliveryDateId: deliveryDateId_example,
  } satisfies DeleteDeliveryDateRequest;

  try {
    const data = await api.deleteDeliveryDate(body);
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
| **deliveryDateId** | `string` |  | [Defaults to `undefined`] |

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


## getDeliveryDate

> DeliveryDate getDeliveryDate(deliveryDateId)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { GetDeliveryDateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // string
    deliveryDateId: deliveryDateId_example,
  } satisfies GetDeliveryDateRequest;

  try {
    const data = await api.getDeliveryDate(body);
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
| **deliveryDateId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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


## getDeliveryPerformance

> any getDeliveryPerformance(page, pageSize, orderNumber, status, from, to)

On-time performance summary: how many promised delivery dates were met within a period.

### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { GetDeliveryPerformanceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    orderNumber: orderNumber_example,
    // string (optional)
    status: status_example,
    // Date | Only dates on or after this date. (optional)
    from: 2013-10-20,
    // Date | Only dates on or before this date. (optional)
    to: 2013-10-20,
  } satisfies GetDeliveryPerformanceRequest;

  try {
    const data = await api.getDeliveryPerformance(body);
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
| **orderNumber** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **from** | `Date` | Only dates on or after this date. | [Optional] [Defaults to `undefined`] |
| **to** | `Date` | Only dates on or before this date. | [Optional] [Defaults to `undefined`] |

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
| **200** | OK |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listDeliveryDates

> Array&lt;DeliveryDate&gt; listDeliveryDates(page, pageSize, orderNumber, status, from, to)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { ListDeliveryDatesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    orderNumber: orderNumber_example,
    // string (optional)
    status: status_example,
    // Date | Only dates on or after this date. (optional)
    from: 2013-10-20,
    // Date | Only dates on or before this date. (optional)
    to: 2013-10-20,
  } satisfies ListDeliveryDatesRequest;

  try {
    const data = await api.listDeliveryDates(body);
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
| **orderNumber** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **from** | `Date` | Only dates on or after this date. | [Optional] [Defaults to `undefined`] |
| **to** | `Date` | Only dates on or before this date. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;DeliveryDate&gt;**](DeliveryDate.md)

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


## updateDeliveryDate

> DeliveryDate updateDeliveryDate(deliveryDateId, body)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { UpdateDeliveryDateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // string
    deliveryDateId: deliveryDateId_example,
    // any
    body: ...,
  } satisfies UpdateDeliveryDateRequest;

  try {
    const data = await api.updateDeliveryDate(body);
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
| **deliveryDateId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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


## updateDeliveryDateStatus

> DeliveryDate updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate)



### Example

```ts
import {
  Configuration,
  DeliveryDateApi,
} from '@simplebilly/api';
import type { UpdateDeliveryDateStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryDateApi(config);

  const body = {
    // string
    deliveryDateId: deliveryDateId_example,
    // DeliveryDateStatusUpdate
    deliveryDateStatusUpdate: ...,
  } satisfies UpdateDeliveryDateStatusRequest;

  try {
    const data = await api.updateDeliveryDateStatus(body);
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
| **deliveryDateId** | `string` |  | [Defaults to `undefined`] |
| **deliveryDateStatusUpdate** | [DeliveryDateStatusUpdate](DeliveryDateStatusUpdate.md) |  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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

