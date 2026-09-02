# KstApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**kstApi**](KstApi.md#kstapi) | **GET** /api/v1/bookkeeping/kst |  |



## kstApi

> KstErgebnis kstApi(year, gewinn)



### Example

```ts
import {
  Configuration,
  KstApi,
} from '@simplebilly/api';
import type { KstApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KstApi(config);

  const body = {
    // number
    year: 56,
    // string (optional)
    gewinn: gewinn_example,
  } satisfies KstApiRequest;

  try {
    const data = await api.kstApi(body);
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
| **gewinn** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**KstErgebnis**](KstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Körperschaftsteuer Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

