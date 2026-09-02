# ServiceAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createServiceAssignment**](ServiceAssignmentApi.md#createserviceassignment) | **POST** /api/v1/service-assignments |  |
| [**deleteServiceAssignment**](ServiceAssignmentApi.md#deleteserviceassignment) | **DELETE** /api/v1/service-assignments/{id} |  |
| [**getServiceAssignment**](ServiceAssignmentApi.md#getserviceassignment) | **GET** /api/v1/service-assignments/{id} |  |
| [**getServiceAssignments**](ServiceAssignmentApi.md#getserviceassignments) | **GET** /api/v1/service-assignments/ |  |
| [**updateServiceAssignment**](ServiceAssignmentApi.md#updateserviceassignment) | **PUT** /api/v1/service-assignments/{id} |  |



## createServiceAssignment

> ServiceAssignment createServiceAssignment(serviceAssignmentCreate)



### Example

```ts
import {
  Configuration,
  ServiceAssignmentApi,
} from '@simplebilly/api';
import type { CreateServiceAssignmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceAssignmentApi(config);

  const body = {
    // ServiceAssignmentCreate
    serviceAssignmentCreate: ...,
  } satisfies CreateServiceAssignmentRequest;

  try {
    const data = await api.createServiceAssignment(body);
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
| **serviceAssignmentCreate** | [ServiceAssignmentCreate](ServiceAssignmentCreate.md) |  | |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

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


## deleteServiceAssignment

> deleteServiceAssignment(id)



### Example

```ts
import {
  Configuration,
  ServiceAssignmentApi,
} from '@simplebilly/api';
import type { DeleteServiceAssignmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceAssignmentApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteServiceAssignmentRequest;

  try {
    const data = await api.deleteServiceAssignment(body);
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


## getServiceAssignment

> ServiceAssignment getServiceAssignment(id)



### Example

```ts
import {
  Configuration,
  ServiceAssignmentApi,
} from '@simplebilly/api';
import type { GetServiceAssignmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceAssignmentApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetServiceAssignmentRequest;

  try {
    const data = await api.getServiceAssignment(body);
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

[**ServiceAssignment**](ServiceAssignment.md)

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


## getServiceAssignments

> Array&lt;ServiceAssignment&gt; getServiceAssignments(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  ServiceAssignmentApi,
} from '@simplebilly/api';
import type { GetServiceAssignmentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceAssignmentApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetServiceAssignmentsRequest;

  try {
    const data = await api.getServiceAssignments(body);
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

[**Array&lt;ServiceAssignment&gt;**](ServiceAssignment.md)

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


## updateServiceAssignment

> ServiceAssignment updateServiceAssignment(id, serviceAssignmentUpdate)



### Example

```ts
import {
  Configuration,
  ServiceAssignmentApi,
} from '@simplebilly/api';
import type { UpdateServiceAssignmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ServiceAssignmentApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ServiceAssignmentUpdate
    serviceAssignmentUpdate: ...,
  } satisfies UpdateServiceAssignmentRequest;

  try {
    const data = await api.updateServiceAssignment(body);
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
| **serviceAssignmentUpdate** | [ServiceAssignmentUpdate](ServiceAssignmentUpdate.md) |  | |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

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

