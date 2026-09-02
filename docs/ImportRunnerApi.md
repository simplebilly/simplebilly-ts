# ImportRunnerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getImportStatus**](ImportRunnerApi.md#getimportstatus) | **GET** /api/v1/import/{job_id} |  |
| [**startImport**](ImportRunnerApi.md#startimport) | **POST** /api/v1/import/start |  |
| [**testImportConnection**](ImportRunnerApi.md#testimportconnection) | **POST** /api/v1/import/test |  |



## getImportStatus

> ImportJobStatus getImportStatus(jobId)



### Example

```ts
import {
  Configuration,
  ImportRunnerApi,
} from '@simplebilly/api';
import type { GetImportStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ImportRunnerApi(config);

  const body = {
    // string
    jobId: jobId_example,
  } satisfies GetImportStatusRequest;

  try {
    const data = await api.getImportStatus(body);
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
| **jobId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ImportJobStatus**](ImportJobStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import job status |  -  |
| **404** | Job not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## startImport

> ImportStartResponse startImport(importStartRequest)



### Example

```ts
import {
  Configuration,
  ImportRunnerApi,
} from '@simplebilly/api';
import type { StartImportRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ImportRunnerApi(config);

  const body = {
    // ImportStartRequest
    importStartRequest: ...,
  } satisfies StartImportRequest;

  try {
    const data = await api.startImport(body);
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
| **importStartRequest** | [ImportStartRequest](ImportStartRequest.md) |  | |

### Return type

[**ImportStartResponse**](ImportStartResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import job queued |  -  |
| **400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## testImportConnection

> ImportTestResponse testImportConnection(importTestRequest)



### Example

```ts
import {
  Configuration,
  ImportRunnerApi,
} from '@simplebilly/api';
import type { TestImportConnectionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ImportRunnerApi(config);

  const body = {
    // ImportTestRequest
    importTestRequest: ...,
  } satisfies TestImportConnectionRequest;

  try {
    const data = await api.testImportConnection(body);
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
| **importTestRequest** | [ImportTestRequest](ImportTestRequest.md) |  | |

### Return type

[**ImportTestResponse**](ImportTestResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection test result |  -  |
| **400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

