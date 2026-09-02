# PaygapApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**paygapAuskunftApi**](PaygapApi.md#paygapauskunftapi) | **GET** /api/v1/bookkeeping/paygap/auskunft/{employee_id} |  |
| [**paygapExportApi**](PaygapApi.md#paygapexportapi) | **GET** /api/v1/bookkeeping/paygap/export |  |
| [**paygapReportApi**](PaygapApi.md#paygapreportapi) | **GET** /api/v1/bookkeeping/paygap/report |  |



## paygapAuskunftApi

> PayGapInfoResponse paygapAuskunftApi(employeeId)



### Example

```ts
import {
  Configuration,
  PaygapApi,
} from '@simplebilly/api';
import type { PaygapAuskunftApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaygapApi(config);

  const body = {
    // string
    employeeId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies PaygapAuskunftApiRequest;

  try {
    const data = await api.paygapAuskunftApi(body);
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
| **employeeId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PayGapInfoResponse**](PayGapInfoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Individual pay information (§ 10-14 EntgTranspG) |  -  |
| **404** | Employee not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## paygapExportApi

> PayGapExportResponse paygapExportApi()



### Example

```ts
import {
  Configuration,
  PaygapApi,
} from '@simplebilly/api';
import type { PaygapExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaygapApi(config);

  try {
    const data = await api.paygapExportApi();
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

[**PayGapExportResponse**](PayGapExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gender pay gap CSV export |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## paygapReportApi

> PayGapReport paygapReportApi()



### Example

```ts
import {
  Configuration,
  PaygapApi,
} from '@simplebilly/api';
import type { PaygapReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaygapApi(config);

  try {
    const data = await api.paygapReportApi();
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

[**PayGapReport**](PayGapReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gender pay gap report (EntgTranspG, EU 2023/970) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

