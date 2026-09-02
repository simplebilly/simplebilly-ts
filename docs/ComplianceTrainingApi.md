# ComplianceTrainingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createComplianceTraining**](ComplianceTrainingApi.md#createcompliancetraining) | **POST** /api/v1/compliance-trainings |  |
| [**deleteComplianceTraining**](ComplianceTrainingApi.md#deletecompliancetraining) | **DELETE** /api/v1/compliance-trainings/{id} |  |
| [**getComplianceTraining**](ComplianceTrainingApi.md#getcompliancetraining) | **GET** /api/v1/compliance-trainings/{id} |  |
| [**getComplianceTrainings**](ComplianceTrainingApi.md#getcompliancetrainings) | **GET** /api/v1/compliance-trainings/ |  |
| [**updateComplianceTraining**](ComplianceTrainingApi.md#updatecompliancetraining) | **PUT** /api/v1/compliance-trainings/{id} |  |



## createComplianceTraining

> ComplianceTraining createComplianceTraining(complianceTrainingCreate)



### Example

```ts
import {
  Configuration,
  ComplianceTrainingApi,
} from '@simplebilly/api';
import type { CreateComplianceTrainingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceTrainingApi(config);

  const body = {
    // ComplianceTrainingCreate
    complianceTrainingCreate: ...,
  } satisfies CreateComplianceTrainingRequest;

  try {
    const data = await api.createComplianceTraining(body);
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
| **complianceTrainingCreate** | [ComplianceTrainingCreate](ComplianceTrainingCreate.md) |  | |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteComplianceTraining

> deleteComplianceTraining(id)



### Example

```ts
import {
  Configuration,
  ComplianceTrainingApi,
} from '@simplebilly/api';
import type { DeleteComplianceTrainingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceTrainingApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteComplianceTrainingRequest;

  try {
    const data = await api.deleteComplianceTraining(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | No Content |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getComplianceTraining

> ComplianceTraining getComplianceTraining(id)



### Example

```ts
import {
  Configuration,
  ComplianceTrainingApi,
} from '@simplebilly/api';
import type { GetComplianceTrainingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceTrainingApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetComplianceTrainingRequest;

  try {
    const data = await api.getComplianceTraining(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getComplianceTrainings

> Array&lt;ComplianceTraining&gt; getComplianceTrainings(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  ComplianceTrainingApi,
} from '@simplebilly/api';
import type { GetComplianceTrainingsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceTrainingApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetComplianceTrainingsRequest;

  try {
    const data = await api.getComplianceTrainings(body);
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
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **includeDeleted** | `boolean` | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ComplianceTraining&gt;**](ComplianceTraining.md)

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


## updateComplianceTraining

> ComplianceTraining updateComplianceTraining(id, complianceTrainingUpdate)



### Example

```ts
import {
  Configuration,
  ComplianceTrainingApi,
} from '@simplebilly/api';
import type { UpdateComplianceTrainingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceTrainingApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ComplianceTrainingUpdate
    complianceTrainingUpdate: ...,
  } satisfies UpdateComplianceTrainingRequest;

  try {
    const data = await api.updateComplianceTraining(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |
| **complianceTrainingUpdate** | [ComplianceTrainingUpdate](ComplianceTrainingUpdate.md) |  | |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

