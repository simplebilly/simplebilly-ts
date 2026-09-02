# StilleApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**stilleExportApi**](StilleApi.md#stilleexportapi) | **GET** /api/v1/bookkeeping/stille/export |  |
| [**stilleReportApi**](StilleApi.md#stillereportapi) | **GET** /api/v1/bookkeeping/stille/report |  |



## stilleExportApi

> StilleExportResponse stilleExportApi(year)



### Example

```ts
import {
  Configuration,
  StilleApi,
} from '@simplebilly/api';
import type { StilleExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StilleApi(config);

  const body = {
    // number
    year: 56,
  } satisfies StilleExportApiRequest;

  try {
    const data = await api.stilleExportApi(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**StilleExportResponse**](StilleExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Stille Beteiligungen als CSV (BOM, Semikolon) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## stilleReportApi

> StilleReport stilleReportApi(year)



### Example

```ts
import {
  Configuration,
  StilleApi,
} from '@simplebilly/api';
import type { StilleReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StilleApi(config);

  const body = {
    // number
    year: 56,
  } satisfies StilleReportApiRequest;

  try {
    const data = await api.stilleReportApi(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**StilleReport**](StilleReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gewinn-/Verlustverteilung an stille Gesellschafter (§§ 230–236 HGB) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

