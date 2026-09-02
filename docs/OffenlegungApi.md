# OffenlegungApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**offenlegungApi**](OffenlegungApi.md#offenlegungapi) | **GET** /api/v1/bookkeeping/offenlegung |  |



## offenlegungApi

> OffenlegungReport offenlegungApi()



### Example

```ts
import {
  Configuration,
  OffenlegungApi,
} from '@simplebilly/api';
import type { OffenlegungApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OffenlegungApi(config);

  try {
    const data = await api.offenlegungApi();
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

[**OffenlegungReport**](OffenlegungReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Offenlegungs-Checkliste (§ 325 HGB) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

