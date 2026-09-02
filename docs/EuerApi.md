# EuerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**euerApi**](EuerApi.md#euerapi) | **GET** /api/v1/bookkeeping/euer |  |
| [**euerKategorienApi**](EuerApi.md#euerkategorienapi) | **GET** /api/v1/bookkeeping/euer/kategorien |  |



## euerApi

> EuerErgebnis euerApi(year)



### Example

```ts
import {
  Configuration,
  EuerApi,
} from '@simplebilly/api';
import type { EuerApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EuerApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EuerApiRequest;

  try {
    const data = await api.euerApi(body);
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

[**EuerErgebnis**](EuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | EÜR Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## euerKategorienApi

> EuerDetailErgebnis euerKategorienApi(year)



### Example

```ts
import {
  Configuration,
  EuerApi,
} from '@simplebilly/api';
import type { EuerKategorienApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EuerApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EuerKategorienApiRequest;

  try {
    const data = await api.euerKategorienApi(body);
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

[**EuerDetailErgebnis**](EuerDetailErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | EÜR mit Kategorie-Aufschlüsselung |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

