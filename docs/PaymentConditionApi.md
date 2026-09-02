# PaymentConditionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listPaymentConditionsApi**](PaymentConditionApi.md#listpaymentconditionsapi) | **GET** /api/v1/payment-conditions |  |



## listPaymentConditionsApi

> Array&lt;PaymentCondition&gt; listPaymentConditionsApi()



### Example

```ts
import {
  Configuration,
  PaymentConditionApi,
} from '@simplebilly/api';
import type { ListPaymentConditionsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentConditionApi(config);

  try {
    const data = await api.listPaymentConditionsApi();
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

[**Array&lt;PaymentCondition&gt;**](PaymentCondition.md)

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

