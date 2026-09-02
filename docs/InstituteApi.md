# InstituteApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**instituteStatusApi**](InstituteApi.md#institutestatusapi) | **GET** /api/v1/bookkeeping/institute/status |  |



## instituteStatusApi

> InstituteStatus instituteStatusApi()



### Example

```ts
import {
  Configuration,
  InstituteApi,
} from '@simplebilly/api';
import type { InstituteStatusApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InstituteApi(config);

  try {
    const data = await api.instituteStatusApi();
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

[**InstituteStatus**](InstituteStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Institut-Status: Fristen und Checkliste (KWG § 26, HGB § 340k/§ 341k, HGB § 325, GwG § 8) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

