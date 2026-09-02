# FristenApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**fristenApi**](FristenApi.md#fristenapi) | **GET** /api/v1/bookkeeping/fristen |  |



## fristenApi

> FristenErgebnis fristenApi(bundesland, voranmeldungsrhythmus, dauerfristverlaengerung, estAktiv, gewstAktiv, monate)



### Example

```ts
import {
  Configuration,
  FristenApi,
} from '@simplebilly/api';
import type { FristenApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new FristenApi(config);

  const body = {
    // string (optional)
    bundesland: bundesland_example,
    // string (optional)
    voranmeldungsrhythmus: voranmeldungsrhythmus_example,
    // boolean (optional)
    dauerfristverlaengerung: true,
    // boolean (optional)
    estAktiv: true,
    // boolean (optional)
    gewstAktiv: true,
    // number (optional)
    monate: 56,
  } satisfies FristenApiRequest;

  try {
    const data = await api.fristenApi(body);
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
| **bundesland** | `string` |  | [Optional] [Defaults to `undefined`] |
| **voranmeldungsrhythmus** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dauerfristverlaengerung** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **estAktiv** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **gewstAktiv** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **monate** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**FristenErgebnis**](FristenErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Steuerliche Fristen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

