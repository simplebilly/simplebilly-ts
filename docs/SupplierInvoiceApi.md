# SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSupplierInvoice**](SupplierInvoiceApi.md#createsupplierinvoice) | **POST** /api/v1/supplier-invoices |  |
| [**deleteSupplierInvoice**](SupplierInvoiceApi.md#deletesupplierinvoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**getSupplierInvoice**](SupplierInvoiceApi.md#getsupplierinvoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**listSupplierInvoices**](SupplierInvoiceApi.md#listsupplierinvoices) | **GET** /api/v1/supplier-invoices/ |  |
| [**updateSupplierInvoice**](SupplierInvoiceApi.md#updatesupplierinvoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**updateSupplierInvoiceStatus**](SupplierInvoiceApi.md#updatesupplierinvoicestatus) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status |  |



## createSupplierInvoice

> SupplierInvoice createSupplierInvoice(supplierInvoice)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { CreateSupplierInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // SupplierInvoice
    supplierInvoice: ...,
  } satisfies CreateSupplierInvoiceRequest;

  try {
    const data = await api.createSupplierInvoice(body);
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
| **supplierInvoice** | [SupplierInvoice](SupplierInvoice.md) |  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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


## deleteSupplierInvoice

> deleteSupplierInvoice(supplierInvoiceId)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { DeleteSupplierInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // string
    supplierInvoiceId: supplierInvoiceId_example,
  } satisfies DeleteSupplierInvoiceRequest;

  try {
    const data = await api.deleteSupplierInvoice(body);
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
| **supplierInvoiceId** | `string` |  | [Defaults to `undefined`] |

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
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSupplierInvoice

> SupplierInvoice getSupplierInvoice(supplierInvoiceId)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { GetSupplierInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // string
    supplierInvoiceId: supplierInvoiceId_example,
  } satisfies GetSupplierInvoiceRequest;

  try {
    const data = await api.getSupplierInvoice(body);
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
| **supplierInvoiceId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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


## listSupplierInvoices

> Array&lt;SupplierInvoice&gt; listSupplierInvoices(page, pageSize, status, purchaseOrderId, supplierName)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { ListSupplierInvoicesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    purchaseOrderId: purchaseOrderId_example,
    // string (optional)
    supplierName: supplierName_example,
  } satisfies ListSupplierInvoicesRequest;

  try {
    const data = await api.listSupplierInvoices(body);
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
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **purchaseOrderId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierName** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;SupplierInvoice&gt;**](SupplierInvoice.md)

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


## updateSupplierInvoice

> SupplierInvoice updateSupplierInvoice(supplierInvoiceId, body)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { UpdateSupplierInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // string
    supplierInvoiceId: supplierInvoiceId_example,
    // any
    body: ...,
  } satisfies UpdateSupplierInvoiceRequest;

  try {
    const data = await api.updateSupplierInvoice(body);
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
| **supplierInvoiceId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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


## updateSupplierInvoiceStatus

> SupplierInvoice updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate)



### Example

```ts
import {
  Configuration,
  SupplierInvoiceApi,
} from '@simplebilly/api';
import type { UpdateSupplierInvoiceStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierInvoiceApi(config);

  const body = {
    // string
    supplierInvoiceId: supplierInvoiceId_example,
    // SupplierInvoiceStatusUpdate
    supplierInvoiceStatusUpdate: ...,
  } satisfies UpdateSupplierInvoiceStatusRequest;

  try {
    const data = await api.updateSupplierInvoiceStatus(body);
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
| **supplierInvoiceId** | `string` |  | [Defaults to `undefined`] |
| **supplierInvoiceStatusUpdate** | [SupplierInvoiceStatusUpdate](SupplierInvoiceStatusUpdate.md) |  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

