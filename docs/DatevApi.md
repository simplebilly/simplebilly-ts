# DatevApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**datevExportApi**](DatevApi.md#datevexportapi) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV |
| [**datevPreviewApi**](DatevApi.md#datevpreviewapi) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review |



## datevExportApi

> DatevExportResponse datevExportApi(accountSchema, dateFrom, dateTo, page, pageSize)

Export bookkeeping data as DATEV CSV

### Example

```ts
import {
  Configuration,
  DatevApi,
} from '@simplebilly/api';
import type { DatevExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DatevApi(config);

  const body = {
    // string (optional)
    accountSchema: accountSchema_example,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies DatevExportApiRequest;

  try {
    const data = await api.datevExportApi(body);
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
| **accountSchema** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**DatevExportResponse**](DatevExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DATEV CSV export |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## datevPreviewApi

> Array&lt;DatevBookingPreview&gt; datevPreviewApi(accountSchema, dateFrom, dateTo, page, pageSize)

Exported_datev_bookings: returns formed bookings for review

### Example

```ts
import {
  Configuration,
  DatevApi,
} from '@simplebilly/api';
import type { DatevPreviewApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DatevApi(config);

  const body = {
    // string (optional)
    accountSchema: accountSchema_example,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies DatevPreviewApiRequest;

  try {
    const data = await api.datevPreviewApi(body);
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
| **accountSchema** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;DatevBookingPreview&gt;**](DatevBookingPreview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DATEV booking preview |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

