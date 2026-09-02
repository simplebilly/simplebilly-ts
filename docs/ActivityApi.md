# ActivityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createActivity**](ActivityApi.md#createactivity) | **POST** /api/v1/activities |  |
| [**deleteActivity**](ActivityApi.md#deleteactivity) | **DELETE** /api/v1/activities/{activity_id} |  |
| [**getActivity**](ActivityApi.md#getactivity) | **GET** /api/v1/activities/{activity_id} |  |
| [**listActivities**](ActivityApi.md#listactivities) | **GET** /api/v1/activities/ |  |
| [**updateActivity**](ActivityApi.md#updateactivity) | **PUT** /api/v1/activities/{activity_id} |  |
| [**updateActivityStatus**](ActivityApi.md#updateactivitystatus) | **PUT** /api/v1/activities/{activity_id}/status |  |



## createActivity

> Activity createActivity(activity)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { CreateActivityRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // Activity
    activity: ...,
  } satisfies CreateActivityRequest;

  try {
    const data = await api.createActivity(body);
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
| **activity** | [Activity](Activity.md) |  | |

### Return type

[**Activity**](Activity.md)

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


## deleteActivity

> deleteActivity(activityId)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { DeleteActivityRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // string
    activityId: activityId_example,
  } satisfies DeleteActivityRequest;

  try {
    const data = await api.deleteActivity(body);
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
| **activityId** | `string` |  | [Defaults to `undefined`] |

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
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getActivity

> Activity getActivity(activityId)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { GetActivityRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // string
    activityId: activityId_example,
  } satisfies GetActivityRequest;

  try {
    const data = await api.getActivity(body);
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
| **activityId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Activity**](Activity.md)

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


## listActivities

> Array&lt;Activity&gt; listActivities(page, pageSize, contactId, activityType, status, assignedTo, overdueOnly)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { ListActivitiesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    contactId: contactId_example,
    // string (optional)
    activityType: activityType_example,
    // string (optional)
    status: status_example,
    // string (optional)
    assignedTo: assignedTo_example,
    // boolean | Only show overdue follow-ups. (optional)
    overdueOnly: true,
  } satisfies ListActivitiesRequest;

  try {
    const data = await api.listActivities(body);
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
| **contactId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **activityType** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **assignedTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **overdueOnly** | `boolean` | Only show overdue follow-ups. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Activity&gt;**](Activity.md)

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


## updateActivity

> Activity updateActivity(activityId, body)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { UpdateActivityRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // string
    activityId: activityId_example,
    // any
    body: ...,
  } satisfies UpdateActivityRequest;

  try {
    const data = await api.updateActivity(body);
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
| **activityId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**Activity**](Activity.md)

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


## updateActivityStatus

> Activity updateActivityStatus(activityId, activityStatusUpdate)



### Example

```ts
import {
  Configuration,
  ActivityApi,
} from '@simplebilly/api';
import type { UpdateActivityStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ActivityApi(config);

  const body = {
    // string
    activityId: activityId_example,
    // ActivityStatusUpdate
    activityStatusUpdate: ...,
  } satisfies UpdateActivityStatusRequest;

  try {
    const data = await api.updateActivityStatus(body);
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
| **activityId** | `string` |  | [Defaults to `undefined`] |
| **activityStatusUpdate** | [ActivityStatusUpdate](ActivityStatusUpdate.md) |  | |

### Return type

[**Activity**](Activity.md)

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

