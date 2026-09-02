# AbsenceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createAbsence**](AbsenceApi.md#createabsence) | **POST** /api/v1/absences |  |
| [**deleteAbsence**](AbsenceApi.md#deleteabsence) | **DELETE** /api/v1/absences/{id} |  |
| [**getAbsence**](AbsenceApi.md#getabsence) | **GET** /api/v1/absences/{id} |  |
| [**getAbsences**](AbsenceApi.md#getabsences) | **GET** /api/v1/absences/ |  |
| [**updateAbsence**](AbsenceApi.md#updateabsence) | **PUT** /api/v1/absences/{id} |  |



## createAbsence

> Absence createAbsence(absenceCreate)



### Example

```ts
import {
  Configuration,
  AbsenceApi,
} from '@simplebilly/api';
import type { CreateAbsenceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AbsenceApi(config);

  const body = {
    // AbsenceCreate
    absenceCreate: ...,
  } satisfies CreateAbsenceRequest;

  try {
    const data = await api.createAbsence(body);
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
| **absenceCreate** | [AbsenceCreate](AbsenceCreate.md) |  | |

### Return type

[**Absence**](Absence.md)

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


## deleteAbsence

> deleteAbsence(id)



### Example

```ts
import {
  Configuration,
  AbsenceApi,
} from '@simplebilly/api';
import type { DeleteAbsenceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AbsenceApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteAbsenceRequest;

  try {
    const data = await api.deleteAbsence(body);
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


## getAbsence

> Absence getAbsence(id)



### Example

```ts
import {
  Configuration,
  AbsenceApi,
} from '@simplebilly/api';
import type { GetAbsenceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AbsenceApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetAbsenceRequest;

  try {
    const data = await api.getAbsence(body);
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

[**Absence**](Absence.md)

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


## getAbsences

> Array&lt;Absence&gt; getAbsences(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  AbsenceApi,
} from '@simplebilly/api';
import type { GetAbsencesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AbsenceApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetAbsencesRequest;

  try {
    const data = await api.getAbsences(body);
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

[**Array&lt;Absence&gt;**](Absence.md)

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


## updateAbsence

> Absence updateAbsence(id, absenceUpdate)



### Example

```ts
import {
  Configuration,
  AbsenceApi,
} from '@simplebilly/api';
import type { UpdateAbsenceRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AbsenceApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // AbsenceUpdate
    absenceUpdate: ...,
  } satisfies UpdateAbsenceRequest;

  try {
    const data = await api.updateAbsence(body);
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
| **absenceUpdate** | [AbsenceUpdate](AbsenceUpdate.md) |  | |

### Return type

[**Absence**](Absence.md)

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

