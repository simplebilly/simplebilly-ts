# DeliveryNoteApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDeliveryNote**](DeliveryNoteApi.md#createdeliverynote) | **POST** /api/v1/delivery-notes |  |
| [**deleteDeliveryNote**](DeliveryNoteApi.md#deletedeliverynote) | **DELETE** /api/v1/delivery-notes/{delivery_note_id} |  |
| [**deliverynoteRestore**](DeliveryNoteApi.md#deliverynoterestore) | **POST** /api/v1/delivery-notes/{delivery_note_id}/restore |  |
| [**downloadDeliveryNotePdf**](DeliveryNoteApi.md#downloaddeliverynotepdf) | **GET** /api/v1/delivery-notes/{delivery_note_id}/pdf |  |
| [**getDeliveryNote**](DeliveryNoteApi.md#getdeliverynote) | **GET** /api/v1/delivery-notes/{delivery_note_id} |  |
| [**listDeliveryNotes**](DeliveryNoteApi.md#listdeliverynotes) | **GET** /api/v1/delivery-notes/ |  |
| [**pursueDeliveryNote**](DeliveryNoteApi.md#pursuedeliverynote) | **POST** /api/v1/delivery-notes/{delivery_note_id}/pursue |  |



## createDeliveryNote

> DeliveryNote createDeliveryNote(deliveryNoteCreate)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { CreateDeliveryNoteRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // DeliveryNoteCreate
    deliveryNoteCreate: ...,
  } satisfies CreateDeliveryNoteRequest;

  try {
    const data = await api.createDeliveryNote(body);
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
| **deliveryNoteCreate** | [DeliveryNoteCreate](DeliveryNoteCreate.md) |  | |

### Return type

[**DeliveryNote**](DeliveryNote.md)

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


## deleteDeliveryNote

> deleteDeliveryNote(deliveryNoteId)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { DeleteDeliveryNoteRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // string
    deliveryNoteId: deliveryNoteId_example,
  } satisfies DeleteDeliveryNoteRequest;

  try {
    const data = await api.deleteDeliveryNote(body);
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
| **deliveryNoteId** | `string` |  | [Defaults to `undefined`] |

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


## deliverynoteRestore

> DeliveryNote deliverynoteRestore(deliveryNoteId)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { DeliverynoteRestoreRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // string
    deliveryNoteId: deliveryNoteId_example,
  } satisfies DeliverynoteRestoreRequest;

  try {
    const data = await api.deliverynoteRestore(body);
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
| **deliveryNoteId** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Restored |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## downloadDeliveryNotePdf

> downloadDeliveryNotePdf(deliveryNoteId)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { DownloadDeliveryNotePdfRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // string
    deliveryNoteId: deliveryNoteId_example,
  } satisfies DownloadDeliveryNotePdfRequest;

  try {
    const data = await api.downloadDeliveryNotePdf(body);
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
| **deliveryNoteId** | `string` |  | [Defaults to `undefined`] |

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


## getDeliveryNote

> DeliveryNote getDeliveryNote(deliveryNoteId)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { GetDeliveryNoteRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // string
    deliveryNoteId: deliveryNoteId_example,
  } satisfies GetDeliveryNoteRequest;

  try {
    const data = await api.getDeliveryNote(body);
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
| **deliveryNoteId** | `string` |  | [Defaults to `undefined`] |

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
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listDeliveryNotes

> Array&lt;DeliveryNote&gt; listDeliveryNotes(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { ListDeliveryNotesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies ListDeliveryNotesRequest;

  try {
    const data = await api.listDeliveryNotes(body);
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

[**Array&lt;DeliveryNote&gt;**](DeliveryNote.md)

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


## pursueDeliveryNote

> Invoice pursueDeliveryNote(deliveryNoteId)



### Example

```ts
import {
  Configuration,
  DeliveryNoteApi,
} from '@simplebilly/api';
import type { PursueDeliveryNoteRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryNoteApi(config);

  const body = {
    // string
    deliveryNoteId: deliveryNoteId_example,
  } satisfies PursueDeliveryNoteRequest;

  try {
    const data = await api.pursueDeliveryNote(body);
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
| **deliveryNoteId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created Invoice |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

