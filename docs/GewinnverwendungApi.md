# GewinnverwendungApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**gewinnverwendungApi**](GewinnverwendungApi.md#gewinnverwendungapi) | **GET** /api/v1/bookkeeping/gewinnverwendung |  |
| [**gewinnverwendungExportApi**](GewinnverwendungApi.md#gewinnverwendungexportapi) | **GET** /api/v1/bookkeeping/gewinnverwendung/export |  |



## gewinnverwendungApi

> GewinnverwendungsReport gewinnverwendungApi(year)



### Example

```ts
import {
  Configuration,
  GewinnverwendungApi,
} from '@simplebilly/api';
import type { GewinnverwendungApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GewinnverwendungApi(config);

  const body = {
    // number
    year: 56,
  } satisfies GewinnverwendungApiRequest;

  try {
    const data = await api.gewinnverwendungApi(body);
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

[**GewinnverwendungsReport**](GewinnverwendungsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gewinnverwendungsrechnung (§ 150, § 174 AktG) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## gewinnverwendungExportApi

> GewinnverwendungsExportResponse gewinnverwendungExportApi(year)



### Example

```ts
import {
  Configuration,
  GewinnverwendungApi,
} from '@simplebilly/api';
import type { GewinnverwendungExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GewinnverwendungApi(config);

  const body = {
    // number
    year: 56,
  } satisfies GewinnverwendungExportApiRequest;

  try {
    const data = await api.gewinnverwendungExportApi(body);
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

[**GewinnverwendungsExportResponse**](GewinnverwendungsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gewinnverwendungsrechnung als CSV (BOM, Semikolon) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

