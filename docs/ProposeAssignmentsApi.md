# ProposeAssignmentsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**proposeAssignmentsApi**](ProposeAssignmentsApi.md#proposeassignmentsapi) | **GET** /api/v1/bookkeeping/propose-assignments |  |



## proposeAssignmentsApi

> Array&lt;ProposedAssignment&gt; proposeAssignmentsApi(minConfidence, customerId)



### Example

```ts
import {
  Configuration,
  ProposeAssignmentsApi,
} from '@simplebilly/api';
import type { ProposeAssignmentsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProposeAssignmentsApi(config);

  const body = {
    // number (optional)
    minConfidence: 1.2,
    // string (optional)
    customerId: customerId_example,
  } satisfies ProposeAssignmentsApiRequest;

  try {
    const data = await api.proposeAssignmentsApi(body);
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
| **minConfidence** | `number` |  | [Optional] [Defaults to `undefined`] |
| **customerId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProposedAssignment&gt;**](ProposedAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Proposed payment to invoice assignments |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

