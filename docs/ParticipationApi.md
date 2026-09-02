# ParticipationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createParticipation**](ParticipationApi.md#createparticipation) | **POST** /api/v1/participations |  |
| [**deleteParticipation**](ParticipationApi.md#deleteparticipation) | **DELETE** /api/v1/participations/{id} |  |
| [**getParticipation**](ParticipationApi.md#getparticipation) | **GET** /api/v1/participations/{id} |  |
| [**getParticipations**](ParticipationApi.md#getparticipations) | **GET** /api/v1/participations/ |  |
| [**updateParticipation**](ParticipationApi.md#updateparticipation) | **PUT** /api/v1/participations/{id} |  |



## createParticipation

> Participation createParticipation(participationCreate)



### Example

```ts
import {
  Configuration,
  ParticipationApi,
} from '@simplebilly/api';
import type { CreateParticipationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ParticipationApi(config);

  const body = {
    // ParticipationCreate
    participationCreate: ...,
  } satisfies CreateParticipationRequest;

  try {
    const data = await api.createParticipation(body);
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
| **participationCreate** | [ParticipationCreate](ParticipationCreate.md) |  | |

### Return type

[**Participation**](Participation.md)

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


## deleteParticipation

> deleteParticipation(id)



### Example

```ts
import {
  Configuration,
  ParticipationApi,
} from '@simplebilly/api';
import type { DeleteParticipationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ParticipationApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteParticipationRequest;

  try {
    const data = await api.deleteParticipation(body);
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


## getParticipation

> Participation getParticipation(id)



### Example

```ts
import {
  Configuration,
  ParticipationApi,
} from '@simplebilly/api';
import type { GetParticipationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ParticipationApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetParticipationRequest;

  try {
    const data = await api.getParticipation(body);
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

[**Participation**](Participation.md)

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


## getParticipations

> Array&lt;Participation&gt; getParticipations(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  ParticipationApi,
} from '@simplebilly/api';
import type { GetParticipationsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ParticipationApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetParticipationsRequest;

  try {
    const data = await api.getParticipations(body);
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

[**Array&lt;Participation&gt;**](Participation.md)

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


## updateParticipation

> Participation updateParticipation(id, participationUpdate)



### Example

```ts
import {
  Configuration,
  ParticipationApi,
} from '@simplebilly/api';
import type { UpdateParticipationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ParticipationApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ParticipationUpdate
    participationUpdate: ...,
  } satisfies UpdateParticipationRequest;

  try {
    const data = await api.updateParticipation(body);
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
| **participationUpdate** | [ParticipationUpdate](ParticipationUpdate.md) |  | |

### Return type

[**Participation**](Participation.md)

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

