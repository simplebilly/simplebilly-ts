# EbilanzApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**ebilanzReportApi**](EbilanzApi.md#ebilanzreportapi) | **GET** /api/v1/bookkeeping/ebilanz |  |
| [**ebilanzXbrlExportApi**](EbilanzApi.md#ebilanzxbrlexportapi) | **GET** /api/v1/bookkeeping/ebilanz/xbrl |  |



## ebilanzReportApi

> EBilanzReport ebilanzReportApi(year, dateFrom, dateTo)



### Example

```ts
import {
  Configuration,
  EbilanzApi,
} from '@simplebilly/api';
import type { EbilanzReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EbilanzApi(config);

  const body = {
    // number (optional)
    year: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
  } satisfies EbilanzReportApiRequest;

  try {
    const data = await api.ebilanzReportApi(body);
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
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**EBilanzReport**](EBilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | E-Bilanz report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## ebilanzXbrlExportApi

> ebilanzXbrlExportApi(year, dateFrom, dateTo)



### Example

```ts
import {
  Configuration,
  EbilanzApi,
} from '@simplebilly/api';
import type { EbilanzXbrlExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EbilanzApi(config);

  const body = {
    // number (optional)
    year: 56,
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
  } satisfies EbilanzXbrlExportApiRequest;

  try {
    const data = await api.ebilanzXbrlExportApi(body);
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
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/xml`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | XBRL XML content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

