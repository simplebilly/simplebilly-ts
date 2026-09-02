# PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPublicReturnStatus**](PublicReturnsApi.md#getpublicreturnstatus) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order\&#39;s email matches. |
| [**listPublicReturns**](PublicReturnsApi.md#listpublicreturns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth). |
| [**requestPublicReturn**](PublicReturnsApi.md#requestpublicreturn) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth). |



## getPublicReturnStatus

> PublicReturnStatusResponse getPublicReturnStatus(email, returnNumber, returnOrderId, orderNumber)

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order\&#39;s email matches.

### Example

```ts
import {
  Configuration,
  PublicReturnsApi,
} from '@simplebilly/api';
import type { GetPublicReturnStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PublicReturnsApi(config);

  const body = {
    // string
    email: email_example,
    // string | Either return_number or return_order_id must be provided. (optional)
    returnNumber: returnNumber_example,
    // string (optional)
    returnOrderId: returnOrderId_example,
    // string (optional)
    orderNumber: orderNumber_example,
  } satisfies GetPublicReturnStatusRequest;

  try {
    const data = await api.getPublicReturnStatus(body);
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
| **email** | `string` |  | [Defaults to `undefined`] |
| **returnNumber** | `string` | Either return_number or return_order_id must be provided. | [Optional] [Defaults to `undefined`] |
| **returnOrderId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **orderNumber** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**PublicReturnStatusResponse**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Return status |  -  |
| **400** | Bad request (missing return identifier) |  -  |
| **404** | Return not found or email mismatch |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPublicReturns

> Array&lt;PublicReturnStatusResponse&gt; listPublicReturns(orderNumber, email)

List all returns for an order (public, no auth).

### Example

```ts
import {
  Configuration,
  PublicReturnsApi,
} from '@simplebilly/api';
import type { ListPublicReturnsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PublicReturnsApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
    // string
    email: email_example,
  } satisfies ListPublicReturnsRequest;

  try {
    const data = await api.listPublicReturns(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |
| **email** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;PublicReturnStatusResponse&gt;**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Returns for the order |  -  |
| **404** | Order not found or email mismatch |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## requestPublicReturn

> PublicReturnResponse requestPublicReturn(publicReturnRequest)

Customer requests a return for an order (public, no auth).

### Example

```ts
import {
  Configuration,
  PublicReturnsApi,
} from '@simplebilly/api';
import type { RequestPublicReturnRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PublicReturnsApi(config);

  const body = {
    // PublicReturnRequest
    publicReturnRequest: ...,
  } satisfies RequestPublicReturnRequest;

  try {
    const data = await api.requestPublicReturn(body);
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
| **publicReturnRequest** | [PublicReturnRequest](PublicReturnRequest.md) |  | |

### Return type

[**PublicReturnResponse**](PublicReturnResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Return requested |  -  |
| **400** | Bad request (item not in order / quantity too high) |  -  |
| **404** | Order not found or email mismatch |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

