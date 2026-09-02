# LeadApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listLeadsApi**](LeadApi.md#listleadsapi) | **GET** /api/v1/support/leads |  |
| [**updateLeadApi**](LeadApi.md#updateleadapi) | **PUT** /api/v1/support/leads/{lead_id} |  |



## listLeadsApi

> Array&lt;Lead&gt; listLeadsApi(status, source, search, page, pageSize)



### Example

```ts
import {
  Configuration,
  LeadApi,
} from '@simplebilly/api';
import type { ListLeadsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LeadApi(config);

  const body = {
    // string (optional)
    status: status_example,
    // string (optional)
    source: source_example,
    // string (optional)
    search: search_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies ListLeadsApiRequest;

  try {
    const data = await api.listLeadsApi(body);
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
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **source** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Lead&gt;**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leads list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateLeadApi

> Lead updateLeadApi(leadId, leadUpdate)



### Example

```ts
import {
  Configuration,
  LeadApi,
} from '@simplebilly/api';
import type { UpdateLeadApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LeadApi(config);

  const body = {
    // string
    leadId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // LeadUpdate
    leadUpdate: ...,
  } satisfies UpdateLeadApiRequest;

  try {
    const data = await api.updateLeadApi(body);
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
| **leadId** | `string` |  | [Defaults to `undefined`] |
| **leadUpdate** | [LeadUpdate](LeadUpdate.md) |  | |

### Return type

[**Lead**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Lead updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

