# GewerbesteuerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**gewerbesteuerApi**](GewerbesteuerApi.md#gewerbesteuerapi) | **GET** /api/v1/bookkeeping/gewerbesteuer |  |



## gewerbesteuerApi

> GewerbesteuerErgebnis gewerbesteuerApi(year, hebesatz, gewerbeertrag, country, gemeindeschluessel)



### Example

```ts
import {
  Configuration,
  GewerbesteuerApi,
} from '@simplebilly/api';
import type { GewerbesteuerApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GewerbesteuerApi(config);

  const body = {
    // number
    year: 56,
    // string (optional)
    hebesatz: hebesatz_example,
    // string (optional)
    gewerbeertrag: gewerbeertrag_example,
    // string (optional)
    country: country_example,
    // string (optional)
    gemeindeschluessel: gemeindeschluessel_example,
  } satisfies GewerbesteuerApiRequest;

  try {
    const data = await api.gewerbesteuerApi(body);
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
| **hebesatz** | `string` |  | [Optional] [Defaults to `undefined`] |
| **gewerbeertrag** | `string` |  | [Optional] [Defaults to `undefined`] |
| **country** | `string` |  | [Optional] [Defaults to `undefined`] |
| **gemeindeschluessel** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**GewerbesteuerErgebnis**](GewerbesteuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gewerbesteuer / Trade Tax Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

