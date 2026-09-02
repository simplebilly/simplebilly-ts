# ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listOpenItemsApi**](ListOpenItemsApi.md#listopenitemsapi) | **GET** /api/v1/bookkeeping/open-items |  |



## listOpenItemsApi

> Array&lt;OpenItem&gt; listOpenItemsApi(reminderLevel1Days, reminderLevel2Days, reminderLevel3Days, customerId)



### Example

```ts
import {
  Configuration,
  ListOpenItemsApi,
} from '@simplebilly/api';
import type { ListOpenItemsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ListOpenItemsApi(config);

  const body = {
    // number (optional)
    reminderLevel1Days: 789,
    // number (optional)
    reminderLevel2Days: 789,
    // number (optional)
    reminderLevel3Days: 789,
    // string (optional)
    customerId: customerId_example,
  } satisfies ListOpenItemsApiRequest;

  try {
    const data = await api.listOpenItemsApi(body);
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
| **reminderLevel1Days** | `number` |  | [Optional] [Defaults to `undefined`] |
| **reminderLevel2Days** | `number` |  | [Optional] [Defaults to `undefined`] |
| **reminderLevel3Days** | `number` |  | [Optional] [Defaults to `undefined`] |
| **customerId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;OpenItem&gt;**](OpenItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of open invoices |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

