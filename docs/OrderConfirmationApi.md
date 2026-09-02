# OrderConfirmationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createConfirmation**](OrderConfirmationApi.md#createconfirmation) | **POST** /api/v1/order-confirmations |  |
| [**deleteConfirmation**](OrderConfirmationApi.md#deleteconfirmation) | **DELETE** /api/v1/order-confirmations/{confirmation_id} |  |
| [**downloadConfirmationPdf**](OrderConfirmationApi.md#downloadconfirmationpdf) | **GET** /api/v1/order-confirmations/{confirmation_id}/pdf |  |
| [**getConfirmation**](OrderConfirmationApi.md#getconfirmation) | **GET** /api/v1/order-confirmations/{confirmation_id} |  |
| [**listConfirmations**](OrderConfirmationApi.md#listconfirmations) | **GET** /api/v1/order-confirmations/ |  |
| [**orderconfirmationRestore**](OrderConfirmationApi.md#orderconfirmationrestore) | **POST** /api/v1/order-confirmations/{confirmation_id}/restore |  |
| [**pursueConfirmation**](OrderConfirmationApi.md#pursueconfirmation) | **POST** /api/v1/order-confirmations/{confirmation_id}/pursue |  |



## createConfirmation

> OrderConfirmation createConfirmation(orderConfirmationCreate)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { CreateConfirmationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // OrderConfirmationCreate
    orderConfirmationCreate: ...,
  } satisfies CreateConfirmationRequest;

  try {
    const data = await api.createConfirmation(body);
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
| **orderConfirmationCreate** | [OrderConfirmationCreate](OrderConfirmationCreate.md) |  | |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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


## deleteConfirmation

> deleteConfirmation(confirmationId)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { DeleteConfirmationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // string
    confirmationId: confirmationId_example,
  } satisfies DeleteConfirmationRequest;

  try {
    const data = await api.deleteConfirmation(body);
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
| **confirmationId** | `string` |  | [Defaults to `undefined`] |

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


## downloadConfirmationPdf

> downloadConfirmationPdf(confirmationId)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { DownloadConfirmationPdfRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // string
    confirmationId: confirmationId_example,
  } satisfies DownloadConfirmationPdfRequest;

  try {
    const data = await api.downloadConfirmationPdf(body);
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
| **confirmationId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/pdf`, `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PDF file |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getConfirmation

> OrderConfirmation getConfirmation(confirmationId)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { GetConfirmationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // string
    confirmationId: confirmationId_example,
  } satisfies GetConfirmationRequest;

  try {
    const data = await api.getConfirmation(body);
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
| **confirmationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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


## listConfirmations

> Array&lt;OrderConfirmation&gt; listConfirmations(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { ListConfirmationsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies ListConfirmationsRequest;

  try {
    const data = await api.listConfirmations(body);
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
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **includeDeleted** | `boolean` | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;OrderConfirmation&gt;**](OrderConfirmation.md)

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


## orderconfirmationRestore

> OrderConfirmation orderconfirmationRestore(confirmationId)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { OrderconfirmationRestoreRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // string
    confirmationId: confirmationId_example,
  } satisfies OrderconfirmationRestoreRequest;

  try {
    const data = await api.orderconfirmationRestore(body);
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
| **confirmationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Restored |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## pursueConfirmation

> DeliveryNote pursueConfirmation(confirmationId)



### Example

```ts
import {
  Configuration,
  OrderConfirmationApi,
} from '@simplebilly/api';
import type { PursueConfirmationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrderConfirmationApi(config);

  const body = {
    // string
    confirmationId: confirmationId_example,
  } satisfies PursueConfirmationRequest;

  try {
    const data = await api.pursueConfirmation(body);
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
| **confirmationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created DeliveryNote |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

