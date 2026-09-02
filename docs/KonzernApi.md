# KonzernApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**konzernExportApi**](KonzernApi.md#konzernexportapi) | **GET** /api/v1/bookkeeping/konzern/status/export |  |
| [**konzernStatusApi**](KonzernApi.md#konzernstatusapi) | **GET** /api/v1/bookkeeping/konzern/status |  |



## konzernExportApi

> KonzernExportResponse konzernExportApi(year)



### Example

```ts
import {
  Configuration,
  KonzernApi,
} from '@simplebilly/api';
import type { KonzernExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KonzernApi(config);

  const body = {
    // number
    year: 56,
  } satisfies KonzernExportApiRequest;

  try {
    const data = await api.konzernExportApi(body);
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

[**KonzernExportResponse**](KonzernExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Konzern-Beteiligungen mit Kontrollstatus als CSV (BOM, Semikolon) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## konzernStatusApi

> KonzernStatus konzernStatusApi(year)



### Example

```ts
import {
  Configuration,
  KonzernApi,
} from '@simplebilly/api';
import type { KonzernStatusApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KonzernApi(config);

  const body = {
    // number
    year: 56,
  } satisfies KonzernStatusApiRequest;

  try {
    const data = await api.konzernStatusApi(body);
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

[**KonzernStatus**](KonzernStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Konzern-Status (§§ 290, 291, 293 HGB) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

