# ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**convertProformaToInvoice**](ProformaInvoiceApi.md#convertproformatoinvoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert |  |
| [**createProformaInvoice**](ProformaInvoiceApi.md#createproformainvoice) | **POST** /api/v1/proforma-invoices |  |
| [**deleteProformaInvoice**](ProformaInvoiceApi.md#deleteproformainvoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} |  |
| [**getProformaInvoice**](ProformaInvoiceApi.md#getproformainvoice) | **GET** /api/v1/proforma-invoices/{proforma_id} |  |
| [**listProformaInvoices**](ProformaInvoiceApi.md#listproformainvoices) | **GET** /api/v1/proforma-invoices/ |  |
| [**updateProformaInvoice**](ProformaInvoiceApi.md#updateproformainvoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} |  |



## convertProformaToInvoice

> ConvertResponse convertProformaToInvoice(proformaId)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { ConvertProformaToInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // string
    proformaId: proformaId_example,
  } satisfies ConvertProformaToInvoiceRequest;

  try {
    const data = await api.convertProformaToInvoice(body);
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
| **proformaId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ConvertResponse**](ConvertResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createProformaInvoice

> ProformaInvoice createProformaInvoice(proformaInvoice)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { CreateProformaInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // ProformaInvoice
    proformaInvoice: ...,
  } satisfies CreateProformaInvoiceRequest;

  try {
    const data = await api.createProformaInvoice(body);
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
| **proformaInvoice** | [ProformaInvoice](ProformaInvoice.md) |  | |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

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


## deleteProformaInvoice

> deleteProformaInvoice(proformaId)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { DeleteProformaInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // string
    proformaId: proformaId_example,
  } satisfies DeleteProformaInvoiceRequest;

  try {
    const data = await api.deleteProformaInvoice(body);
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
| **proformaId** | `string` |  | [Defaults to `undefined`] |

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


## getProformaInvoice

> ProformaInvoice getProformaInvoice(proformaId)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { GetProformaInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // string
    proformaId: proformaId_example,
  } satisfies GetProformaInvoiceRequest;

  try {
    const data = await api.getProformaInvoice(body);
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
| **proformaId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

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


## listProformaInvoices

> Array&lt;ProformaInvoice&gt; listProformaInvoices(page, pageSize, status, customerId, orderNumber)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { ListProformaInvoicesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    customerId: customerId_example,
    // string (optional)
    orderNumber: orderNumber_example,
  } satisfies ListProformaInvoicesRequest;

  try {
    const data = await api.listProformaInvoices(body);
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
| **customerId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **orderNumber** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProformaInvoice&gt;**](ProformaInvoice.md)

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


## updateProformaInvoice

> ProformaInvoice updateProformaInvoice(proformaId, body)



### Example

```ts
import {
  Configuration,
  ProformaInvoiceApi,
} from '@simplebilly/api';
import type { UpdateProformaInvoiceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProformaInvoiceApi(config);

  const body = {
    // string
    proformaId: proformaId_example,
    // any
    body: ...,
  } satisfies UpdateProformaInvoiceRequest;

  try {
    const data = await api.updateProformaInvoice(body);
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
| **proformaId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

