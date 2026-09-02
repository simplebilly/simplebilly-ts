# DownPaymentInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**downloadDownPaymentInvoicePdf**](DownPaymentInvoiceApi.md#downloaddownpaymentinvoicepdf) | **GET** /api/v1/down-payment-invoices/{id}/pdf |  |
| [**getDownPaymentInvoice**](DownPaymentInvoiceApi.md#getdownpaymentinvoice) | **GET** /api/v1/down-payment-invoices/{id} |  |
| [**listDownPaymentInvoices**](DownPaymentInvoiceApi.md#listdownpaymentinvoices) | **GET** /api/v1/down-payment-invoices/ |  |



## downloadDownPaymentInvoicePdf

> downloadDownPaymentInvoicePdf(id)



### Example

```ts
import {
  Configuration,
  DownPaymentInvoiceApi,
} from '@simplebilly/api';
import type { DownloadDownPaymentInvoicePdfRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DownPaymentInvoiceApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies DownloadDownPaymentInvoicePdfRequest;

  try {
    const data = await api.downloadDownPaymentInvoicePdf(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

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
| **200** | PDF placeholder |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getDownPaymentInvoice

> DownPaymentInvoice getDownPaymentInvoice(id)



### Example

```ts
import {
  Configuration,
  DownPaymentInvoiceApi,
} from '@simplebilly/api';
import type { GetDownPaymentInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DownPaymentInvoiceApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies GetDownPaymentInvoiceRequest;

  try {
    const data = await api.getDownPaymentInvoice(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

[**DownPaymentInvoice**](DownPaymentInvoice.md)

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


## listDownPaymentInvoices

> Array&lt;DownPaymentInvoice&gt; listDownPaymentInvoices(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  DownPaymentInvoiceApi,
} from '@simplebilly/api';
import type { ListDownPaymentInvoicesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DownPaymentInvoiceApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies ListDownPaymentInvoicesRequest;

  try {
    const data = await api.listDownPaymentInvoices(body);
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

[**Array&lt;DownPaymentInvoice&gt;**](DownPaymentInvoice.md)

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

