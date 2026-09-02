# KostenVorschauApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**kostenVorschauApi**](KostenVorschauApi.md#kostenvorschauapi) | **GET** /api/v1/bookkeeping/kosten-vorschau |  |



## kostenVorschauApi

> KostenVorschau kostenVorschauApi(year, month)



### Example

```ts
import {
  Configuration,
  KostenVorschauApi,
} from '@simplebilly/api';
import type { KostenVorschauApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KostenVorschauApi(config);

  const body = {
    // number
    year: 56,
    // number
    month: 56,
  } satisfies KostenVorschauApiRequest;

  try {
    const data = await api.kostenVorschauApi(body);
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
| **month** | `number` |  | [Defaults to `undefined`] |

### Return type

[**KostenVorschau**](KostenVorschau.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Kosten-Vorschau für den Monat |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

