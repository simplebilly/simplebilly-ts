# PackingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**completePacking**](PackingApi.md#completepacking) | **POST** /api/v1/packing/{order_number}/complete | Mark packing as complete and transition order to shipped |
| [**getPackingQueue**](PackingApi.md#getpackingqueue) | **GET** /api/v1/packing/queue | Get the packing queue - orders ready for packing |
| [**printDeliveryNote**](PackingApi.md#printdeliverynote) | **POST** /api/v1/packing/{order_number}/print-delivery-note | Print delivery note (Lieferschein) for an order |
| [**printLabel**](PackingApi.md#printlabel) | **POST** /api/v1/packing/{order_number}/print-label | Print shipping label for an order |
| [**recordPackingVideo**](PackingApi.md#recordpackingvideo) | **POST** /api/v1/packing/{order_number}/record-video | Record video of packing process |



## completePacking

> PackingCompleteResponse completePacking(orderNumber, packingCompleteRequest)

Mark packing as complete and transition order to shipped

### Example

```ts
import {
  Configuration,
  PackingApi,
} from '@simplebilly/api';
import type { CompletePackingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PackingApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
    // PackingCompleteRequest
    packingCompleteRequest: ...,
  } satisfies CompletePackingRequest;

  try {
    const data = await api.completePacking(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |
| **packingCompleteRequest** | [PackingCompleteRequest](PackingCompleteRequest.md) |  | |

### Return type

[**PackingCompleteResponse**](PackingCompleteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Packing completed |  -  |
| **404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getPackingQueue

> PackingQueue getPackingQueue(page, pageSize, search)

Get the packing queue - orders ready for packing

### Example

```ts
import {
  Configuration,
  PackingApi,
} from '@simplebilly/api';
import type { GetPackingQueueRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PackingApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
  } satisfies GetPackingQueueRequest;

  try {
    const data = await api.getPackingQueue(body);
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

### Return type

[**PackingQueue**](PackingQueue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Packing queue |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## printDeliveryNote

> PrintDeliveryNoteResponse printDeliveryNote(orderNumber)

Print delivery note (Lieferschein) for an order

### Example

```ts
import {
  Configuration,
  PackingApi,
} from '@simplebilly/api';
import type { PrintDeliveryNoteRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PackingApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
  } satisfies PrintDeliveryNoteRequest;

  try {
    const data = await api.printDeliveryNote(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PrintDeliveryNoteResponse**](PrintDeliveryNoteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Delivery note printed |  -  |
| **404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## printLabel

> PrintLabelResponse printLabel(orderNumber)

Print shipping label for an order

### Example

```ts
import {
  Configuration,
  PackingApi,
} from '@simplebilly/api';
import type { PrintLabelRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PackingApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
  } satisfies PrintLabelRequest;

  try {
    const data = await api.printLabel(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PrintLabelResponse**](PrintLabelResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Label printed |  -  |
| **404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## recordPackingVideo

> PackingVideoResponse recordPackingVideo(orderNumber, body)

Record video of packing process

### Example

```ts
import {
  Configuration,
  PackingApi,
} from '@simplebilly/api';
import type { RecordPackingVideoRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PackingApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
    // any
    body: ...,
  } satisfies RecordPackingVideoRequest;

  try {
    const data = await api.recordPackingVideo(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**PackingVideoResponse**](PackingVideoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Video recorded |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

