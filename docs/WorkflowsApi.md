# WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listWorkflowsApi**](WorkflowsApi.md#listworkflowsapi) | **GET** /api/v1/workflows |  |
| [**setWorkflowEnabledApi**](WorkflowsApi.md#setworkflowenabledapi) | **PUT** /api/v1/workflows/{workflow_id}/enabled |  |



## listWorkflowsApi

> Array&lt;Workflow&gt; listWorkflowsApi()



### Example

```ts
import {
  Configuration,
  WorkflowsApi,
} from '@simplebilly/api';
import type { ListWorkflowsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WorkflowsApi(config);

  try {
    const data = await api.listWorkflowsApi();
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

[**Array&lt;Workflow&gt;**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Workflows (seeded with defaults on first access) |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setWorkflowEnabledApi

> Workflow setWorkflowEnabledApi(workflowId, workflowEnabledUpdate)



### Example

```ts
import {
  Configuration,
  WorkflowsApi,
} from '@simplebilly/api';
import type { SetWorkflowEnabledApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WorkflowsApi(config);

  const body = {
    // string
    workflowId: workflowId_example,
    // WorkflowEnabledUpdate
    workflowEnabledUpdate: ...,
  } satisfies SetWorkflowEnabledApiRequest;

  try {
    const data = await api.setWorkflowEnabledApi(body);
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
| **workflowId** | `string` |  | [Defaults to `undefined`] |
| **workflowEnabledUpdate** | [WorkflowEnabledUpdate](WorkflowEnabledUpdate.md) |  | |

### Return type

[**Workflow**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Workflow enabled state updated |  -  |
| **404** | Workflow not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

