# SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**shippingSuitabilityApi**](SuitabilityApi.md#shippingsuitabilityapi) | **POST** /api/v1/shipping/suitability |  |



## shippingSuitabilityApi

> SuitabilityResult shippingSuitabilityApi(suitabilityRequest)



### Example

```ts
import {
  Configuration,
  SuitabilityApi,
} from '@simplebilly/api';
import type { ShippingSuitabilityApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SuitabilityApi(config);

  const body = {
    // SuitabilityRequest
    suitabilityRequest: ...,
  } satisfies ShippingSuitabilityApiRequest;

  try {
    const data = await api.shippingSuitabilityApi(body);
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
| **suitabilityRequest** | [SuitabilityRequest](SuitabilityRequest.md) |  | |

### Return type

[**SuitabilityResult**](SuitabilityResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Shipping suitability results |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

