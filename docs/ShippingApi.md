# ShippingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getCredentialsApi**](ShippingApi.md#getcredentialsapi) | **GET** /api/v1/shipping/credentials |  |
| [**getRatesApi**](ShippingApi.md#getratesapi) | **POST** /api/v1/shipping/rates |  |
| [**listProvidersApi**](ShippingApi.md#listprovidersapi) | **GET** /api/v1/shipping/providers |  |
| [**saveCredentialsApi**](ShippingApi.md#savecredentialsapi) | **PUT** /api/v1/shipping/credentials |  |



## getCredentialsApi

> ShippingCredentials getCredentialsApi()



### Example

```ts
import {
  Configuration,
  ShippingApi,
} from '@simplebilly/api';
import type { GetCredentialsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingApi(config);

  try {
    const data = await api.getCredentialsApi();
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

[**ShippingCredentials**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Configured shipping provider credentials |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRatesApi

> RateResponse getRatesApi(rateRequest)



### Example

```ts
import {
  Configuration,
  ShippingApi,
} from '@simplebilly/api';
import type { GetRatesApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingApi(config);

  const body = {
    // RateRequest
    rateRequest: ...,
  } satisfies GetRatesApiRequest;

  try {
    const data = await api.getRatesApi(body);
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
| **rateRequest** | [RateRequest](RateRequest.md) |  | |

### Return type

[**RateResponse**](RateResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Shipping rates from configured providers |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listProvidersApi

> Array&lt;ProviderInfo&gt; listProvidersApi()



### Example

```ts
import {
  Configuration,
  ShippingApi,
} from '@simplebilly/api';
import type { ListProvidersApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingApi(config);

  try {
    const data = await api.listProvidersApi();
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

[**Array&lt;ProviderInfo&gt;**](ProviderInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of shipping providers |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## saveCredentialsApi

> ShippingCredentials saveCredentialsApi(shippingCredentials)



### Example

```ts
import {
  Configuration,
  ShippingApi,
} from '@simplebilly/api';
import type { SaveCredentialsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingApi(config);

  const body = {
    // ShippingCredentials
    shippingCredentials: ...,
  } satisfies SaveCredentialsApiRequest;

  try {
    const data = await api.saveCredentialsApi(body);
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
| **shippingCredentials** | [ShippingCredentials](ShippingCredentials.md) |  | |

### Return type

[**ShippingCredentials**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Saved shipping provider credentials |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

