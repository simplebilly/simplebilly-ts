# PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPaymentGatewayApi**](PaymentGatewayApi.md#createpaymentgatewayapi) | **POST** /api/v1/payment-gateways |  |
| [**deletePaymentGatewayApi**](PaymentGatewayApi.md#deletepaymentgatewayapi) | **DELETE** /api/v1/payment-gateways/{gateway_id} |  |
| [**listPaymentGatewaysApi**](PaymentGatewayApi.md#listpaymentgatewaysapi) | **GET** /api/v1/payment-gateways/ |  |
| [**oauthAuthorizeApi**](PaymentGatewayApi.md#oauthauthorizeapi) | **POST** /api/v1/payment-gateways/oauth/authorize |  |
| [**oauthCallbackApi**](PaymentGatewayApi.md#oauthcallbackapi) | **POST** /api/v1/payment-gateways/oauth/callback |  |
| [**updatePaymentGatewayApi**](PaymentGatewayApi.md#updatepaymentgatewayapi) | **PUT** /api/v1/payment-gateways/{gateway_id} |  |



## createPaymentGatewayApi

> PaymentGateway createPaymentGatewayApi(body)



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { CreatePaymentGatewayApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  const body = {
    // any
    body: ...,
  } satisfies CreatePaymentGatewayApiRequest;

  try {
    const data = await api.createPaymentGatewayApi(body);
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
| **body** | `any` |  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deletePaymentGatewayApi

> deletePaymentGatewayApi(gatewayId)



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { DeletePaymentGatewayApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  const body = {
    // string
    gatewayId: gatewayId_example,
  } satisfies DeletePaymentGatewayApiRequest;

  try {
    const data = await api.deletePaymentGatewayApi(body);
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
| **gatewayId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deleted |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPaymentGatewaysApi

> Array&lt;PaymentGateway&gt; listPaymentGatewaysApi()



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { ListPaymentGatewaysApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  try {
    const data = await api.listPaymentGatewaysApi();
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

[**Array&lt;PaymentGateway&gt;**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## oauthAuthorizeApi

> GatewayOAuthAuthorizeResponse oauthAuthorizeApi(gatewayOAuthAuthorizeRequest)



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { OauthAuthorizeApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  const body = {
    // GatewayOAuthAuthorizeRequest
    gatewayOAuthAuthorizeRequest: ...,
  } satisfies OauthAuthorizeApiRequest;

  try {
    const data = await api.oauthAuthorizeApi(body);
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
| **gatewayOAuthAuthorizeRequest** | [GatewayOAuthAuthorizeRequest](GatewayOAuthAuthorizeRequest.md) |  | |

### Return type

[**GatewayOAuthAuthorizeResponse**](GatewayOAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth authorization URL |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## oauthCallbackApi

> PaymentGateway oauthCallbackApi(gatewayOAuthCallbackRequest)



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { OauthCallbackApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  const body = {
    // GatewayOAuthCallbackRequest
    gatewayOAuthCallbackRequest: ...,
  } satisfies OauthCallbackApiRequest;

  try {
    const data = await api.oauthCallbackApi(body);
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
| **gatewayOAuthCallbackRequest** | [GatewayOAuthCallbackRequest](GatewayOAuthCallbackRequest.md) |  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Gateway connected |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updatePaymentGatewayApi

> PaymentGateway updatePaymentGatewayApi(gatewayId, body)



### Example

```ts
import {
  Configuration,
  PaymentGatewayApi,
} from '@simplebilly/api';
import type { UpdatePaymentGatewayApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentGatewayApi(config);

  const body = {
    // string
    gatewayId: gatewayId_example,
    // any
    body: ...,
  } satisfies UpdatePaymentGatewayApiRequest;

  try {
    const data = await api.updatePaymentGatewayApi(body);
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
| **gatewayId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

