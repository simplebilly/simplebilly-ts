# UstvaApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**jahresustApi**](UstvaApi.md#jahresustapi) | **GET** /api/v1/bookkeeping/jahresust |  |
| [**ustvaApi**](UstvaApi.md#ustvaapi) | **GET** /api/v1/bookkeeping/ustva |  |



## jahresustApi

> JahresUstErgebnis jahresustApi(year)



### Example

```ts
import {
  Configuration,
  UstvaApi,
} from '@simplebilly/api';
import type { JahresustApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UstvaApi(config);

  const body = {
    // number
    year: 56,
  } satisfies JahresustApiRequest;

  try {
    const data = await api.jahresustApi(body);
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

[**JahresUstErgebnis**](JahresUstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Jahresumsatzsteuer Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## ustvaApi

> UstvaErgebnis ustvaApi(zeitraum)



### Example

```ts
import {
  Configuration,
  UstvaApi,
} from '@simplebilly/api';
import type { UstvaApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UstvaApi(config);

  const body = {
    // string
    zeitraum: zeitraum_example,
  } satisfies UstvaApiRequest;

  try {
    const data = await api.ustvaApi(body);
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
| **zeitraum** | `string` |  | [Defaults to `undefined`] |

### Return type

[**UstvaErgebnis**](UstvaErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UStVA Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

