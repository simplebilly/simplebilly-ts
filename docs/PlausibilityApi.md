# PlausibilityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**plausibilityCheckApi**](PlausibilityApi.md#plausibilitycheckapi) | **GET** /api/v1/bookkeeping/plausibility |  |



## plausibilityCheckApi

> PlausibilityReport plausibilityCheckApi(dateFrom, dateTo)



### Example

```ts
import {
  Configuration,
  PlausibilityApi,
} from '@simplebilly/api';
import type { PlausibilityCheckApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PlausibilityApi(config);

  const body = {
    // string (optional)
    dateFrom: dateFrom_example,
    // string (optional)
    dateTo: dateTo_example,
  } satisfies PlausibilityCheckApiRequest;

  try {
    const data = await api.plausibilityCheckApi(body);
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
| **dateFrom** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**PlausibilityReport**](PlausibilityReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Plausibility report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

