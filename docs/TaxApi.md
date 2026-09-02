# TaxApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTaxRate**](TaxApi.md#createtaxrate) | **POST** /api/v1/tax-rates | Create a tax rate (&#x60;admin:settings&#x60;). |
| [**deleteTaxRate**](TaxApi.md#deletetaxrate) | **DELETE** /api/v1/tax-rates/{id} | Delete a tax rate by id (&#x60;admin:settings&#x60;). |
| [**listTaxRates**](TaxApi.md#listtaxrates) | **GET** /api/v1/tax-rates | List the calling tenant\&#39;s tax rates. |
| [**updateTaxRate**](TaxApi.md#updatetaxrate) | **PUT** /api/v1/tax-rates/{id} | Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields. |



## createTaxRate

> createTaxRate(taxRateCreate)

Create a tax rate (&#x60;admin:settings&#x60;).

### Example

```ts
import {
  Configuration,
  TaxApi,
} from '@simplebilly/api';
import type { CreateTaxRateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TaxApi(config);

  const body = {
    // TaxRateCreate
    taxRateCreate: ...,
  } satisfies CreateTaxRateRequest;

  try {
    const data = await api.createTaxRate(body);
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
| **taxRateCreate** | [TaxRateCreate](TaxRateCreate.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tax rate created |  -  |
| **400** | Invalid body |  -  |
| **403** | Missing admin:settings permission |  -  |
| **409** | Default rate for the country already exists |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTaxRate

> deleteTaxRate(id)

Delete a tax rate by id (&#x60;admin:settings&#x60;).

### Example

```ts
import {
  Configuration,
  TaxApi,
} from '@simplebilly/api';
import type { DeleteTaxRateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TaxApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteTaxRateRequest;

  try {
    const data = await api.deleteTaxRate(body);
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
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tax rate deleted |  -  |
| **403** | Missing admin:settings permission |  -  |
| **404** | Tax rate not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTaxRates

> listTaxRates()

List the calling tenant\&#39;s tax rates.

### Example

```ts
import {
  Configuration,
  TaxApi,
} from '@simplebilly/api';
import type { ListTaxRatesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TaxApi(config);

  try {
    const data = await api.listTaxRates();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant\&#39;s tax rates |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTaxRate

> updateTaxRate(id, taxRateCreate)

Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.

### Example

```ts
import {
  Configuration,
  TaxApi,
} from '@simplebilly/api';
import type { UpdateTaxRateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TaxApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // TaxRateCreate
    taxRateCreate: ...,
  } satisfies UpdateTaxRateRequest;

  try {
    const data = await api.updateTaxRate(body);
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
| **taxRateCreate** | [TaxRateCreate](TaxRateCreate.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tax rate updated |  -  |
| **400** | Invalid body |  -  |
| **403** | Missing admin:settings permission |  -  |
| **404** | Tax rate not found |  -  |
| **409** | Default rate for the country already exists |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

