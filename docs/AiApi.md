# AiApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aiSuggestApi**](AiApi.md#aisuggestapi) | **POST** /api/v1/support/ai/suggest |  |
| [**createWorkerApi**](AiApi.md#createworkerapi) | **POST** /api/v1/support/ai/workers |  |
| [**listWorkersApi**](AiApi.md#listworkersapi) | **GET** /api/v1/support/ai/workers |  |
| [**runWorkerApi**](AiApi.md#runworkerapi) | **POST** /api/v1/support/ai/workers/{worker_id}/run |  |



## aiSuggestApi

> AiSuggestion aiSuggestApi(aiSuggestionRequest)



### Example

```ts
import {
  Configuration,
  AiApi,
} from '@simplebilly/api';
import type { AiSuggestApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AiApi(config);

  const body = {
    // AiSuggestionRequest
    aiSuggestionRequest: ...,
  } satisfies AiSuggestApiRequest;

  try {
    const data = await api.aiSuggestApi(body);
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
| **aiSuggestionRequest** | [AiSuggestionRequest](AiSuggestionRequest.md) |  | |

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AI suggestion |  -  |
| **500** | AI error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createWorkerApi

> AiWorkerConfig createWorkerApi(aiConfigDto)



### Example

```ts
import {
  Configuration,
  AiApi,
} from '@simplebilly/api';
import type { CreateWorkerApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AiApi(config);

  const body = {
    // AiConfigDto
    aiConfigDto: ...,
  } satisfies CreateWorkerApiRequest;

  try {
    const data = await api.createWorkerApi(body);
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
| **aiConfigDto** | [AiConfigDto](AiConfigDto.md) |  | |

### Return type

[**AiWorkerConfig**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Worker created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listWorkersApi

> Array&lt;AiWorkerConfig&gt; listWorkersApi()



### Example

```ts
import {
  Configuration,
  AiApi,
} from '@simplebilly/api';
import type { ListWorkersApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AiApi(config);

  try {
    const data = await api.listWorkersApi();
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

[**Array&lt;AiWorkerConfig&gt;**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List AI workers |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## runWorkerApi

> AiSuggestion runWorkerApi(workerId, aiSuggestionRequest)



### Example

```ts
import {
  Configuration,
  AiApi,
} from '@simplebilly/api';
import type { RunWorkerApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AiApi(config);

  const body = {
    // string
    workerId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // AiSuggestionRequest
    aiSuggestionRequest: ...,
  } satisfies RunWorkerApiRequest;

  try {
    const data = await api.runWorkerApi(body);
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
| **workerId** | `string` |  | [Defaults to `undefined`] |
| **aiSuggestionRequest** | [AiSuggestionRequest](AiSuggestionRequest.md) |  | |

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Worker executed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

