# AnlageEksApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**eksApi**](AnlageEksApi.md#eksapi) | **GET** /api/v1/bookkeeping/eks |  |



## eksApi

> EksErgebnis eksApi(year)



### Example

```ts
import {
  Configuration,
  AnlageEksApi,
} from '@simplebilly/api';
import type { EksApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AnlageEksApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EksApiRequest;

  try {
    const data = await api.eksApi(body);
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

[**EksErgebnis**](EksErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Anlage EKS Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

