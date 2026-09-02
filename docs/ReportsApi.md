# ReportsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bilanzReportApi**](ReportsApi.md#bilanzreportapi) | **GET** /api/v1/bookkeeping/reports/bilanz | Bilanz (Balance Sheet) |
| [**guvReportApi**](ReportsApi.md#guvreportapi) | **GET** /api/v1/bookkeeping/reports/guv | Gewinn- und Verlustrechnung (P&amp;L statement) |
| [**kontenansichtReportApi**](ReportsApi.md#kontenansichtreportapi) | **GET** /api/v1/bookkeeping/reports/kontenansicht | Kontenansicht (Account Overview) |
| [**umsatzsteuerReportApi**](ReportsApi.md#umsatzsteuerreportapi) | **GET** /api/v1/bookkeeping/reports/umsatzsteuer | Umsatzsteuer-Voranmeldung (VAT report) |



## bilanzReportApi

> BilanzReport bilanzReportApi(year, month, dateFrom, dateTo, page, pageSize)

Bilanz (Balance Sheet)

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@simplebilly/api';
import type { BilanzReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReportsApi(config);

  const body = {
    // number (optional)
    year: 56,
    // number (optional)
    month: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies BilanzReportApiRequest;

  try {
    const data = await api.bilanzReportApi(body);
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
| **year** | `number` |  | [Optional] [Defaults to `undefined`] |
| **month** | `number` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**BilanzReport**](BilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Balance sheet |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## guvReportApi

> GuVReport guvReportApi(year, month, dateFrom, dateTo, page, pageSize)

Gewinn- und Verlustrechnung (P&amp;L statement)

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@simplebilly/api';
import type { GuvReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReportsApi(config);

  const body = {
    // number (optional)
    year: 56,
    // number (optional)
    month: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies GuvReportApiRequest;

  try {
    const data = await api.guvReportApi(body);
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
| **year** | `number` |  | [Optional] [Defaults to `undefined`] |
| **month** | `number` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**GuVReport**](GuVReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GuV report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## kontenansichtReportApi

> KontoReport kontenansichtReportApi(year, month, dateFrom, dateTo, page, pageSize)

Kontenansicht (Account Overview)

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@simplebilly/api';
import type { KontenansichtReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReportsApi(config);

  const body = {
    // number (optional)
    year: 56,
    // number (optional)
    month: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies KontenansichtReportApiRequest;

  try {
    const data = await api.kontenansichtReportApi(body);
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
| **year** | `number` |  | [Optional] [Defaults to `undefined`] |
| **month** | `number` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**KontoReport**](KontoReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Account overview |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## umsatzsteuerReportApi

> UmsatzsteuerReport umsatzsteuerReportApi(year, month, dateFrom, dateTo, page, pageSize)

Umsatzsteuer-Voranmeldung (VAT report)

### Example

```ts
import {
  Configuration,
  ReportsApi,
} from '@simplebilly/api';
import type { UmsatzsteuerReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ReportsApi(config);

  const body = {
    // number (optional)
    year: 56,
    // number (optional)
    month: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies UmsatzsteuerReportApiRequest;

  try {
    const data = await api.umsatzsteuerReportApi(body);
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
| **year** | `number` |  | [Optional] [Defaults to `undefined`] |
| **month** | `number` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**UmsatzsteuerReport**](UmsatzsteuerReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | VAT report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

