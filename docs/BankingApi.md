# BankingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bankLookupApi**](BankingApi.md#banklookupapi) | **GET** /api/v1/bookkeeping/banking/lookup |  |
| [**bankTransactionsApi**](BankingApi.md#banktransactionsapi) | **GET** /api/v1/bookkeeping/banking/transactions |  |
| [**hebesatzLookupApi**](BankingApi.md#hebesatzlookupapi) | **GET** /api/v1/bookkeeping/hebesatz |  |



## bankLookupApi

> BankLookup bankLookupApi(iban)



### Example

```ts
import {
  Configuration,
  BankingApi,
} from '@simplebilly/api';
import type { BankLookupApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BankingApi(config);

  const body = {
    // string
    iban: iban_example,
  } satisfies BankLookupApiRequest;

  try {
    const data = await api.bankLookupApi(body);
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
| **iban** | `string` |  | [Defaults to `undefined`] |

### Return type

[**BankLookup**](BankLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bank-Lookup Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## bankTransactionsApi

> bankTransactionsApi()



### Example

```ts
import {
  Configuration,
  BankingApi,
} from '@simplebilly/api';
import type { BankTransactionsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BankingApi(config);

  try {
    const data = await api.bankTransactionsApi();
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

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bank-Transaktionen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## hebesatzLookupApi

> Array&lt;HebesatzLookup&gt; hebesatzLookupApi(gemeindeschluessel, plz, name, stichtag, countryCode)



### Example

```ts
import {
  Configuration,
  BankingApi,
} from '@simplebilly/api';
import type { HebesatzLookupApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BankingApi(config);

  const body = {
    // string (optional)
    gemeindeschluessel: gemeindeschluessel_example,
    // string (optional)
    plz: plz_example,
    // string (optional)
    name: name_example,
    // string | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from <= date <= valid_to. (optional)
    stichtag: stichtag_example,
    // string (optional)
    countryCode: countryCode_example,
  } satisfies HebesatzLookupApiRequest;

  try {
    const data = await api.hebesatzLookupApi(body);
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
| **gemeindeschluessel** | `string` |  | [Optional] [Defaults to `undefined`] |
| **plz** | `string` |  | [Optional] [Defaults to `undefined`] |
| **name** | `string` |  | [Optional] [Defaults to `undefined`] |
| **stichtag** | `string` | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [Optional] [Defaults to `undefined`] |
| **countryCode** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;HebesatzLookup&gt;**](HebesatzLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Hebesatz Lookup |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

