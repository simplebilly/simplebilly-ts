# EventSubscriptionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEventSubscription**](EventSubscriptionApi.md#createeventsubscription) | **POST** /api/v1/event-subscriptions |  |
| [**deleteEventSubscription**](EventSubscriptionApi.md#deleteeventsubscription) | **DELETE** /api/v1/event-subscriptions/{subscription_id} |  |
| [**listEventSubscriptions**](EventSubscriptionApi.md#listeventsubscriptions) | **GET** /api/v1/event-subscriptions/ |  |



## createEventSubscription

> EventSubscription createEventSubscription(body)



### Example

```ts
import {
  Configuration,
  EventSubscriptionApi,
} from '@simplebilly/api';
import type { CreateEventSubscriptionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventSubscriptionApi(config);

  const body = {
    // any
    body: ...,
  } satisfies CreateEventSubscriptionRequest;

  try {
    const data = await api.createEventSubscription(body);
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
| **body** | `any` |  | |

### Return type

[**EventSubscription**](EventSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **404** | Connection not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteEventSubscription

> deleteEventSubscription(subscriptionId)



### Example

```ts
import {
  Configuration,
  EventSubscriptionApi,
} from '@simplebilly/api';
import type { DeleteEventSubscriptionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventSubscriptionApi(config);

  const body = {
    // string
    subscriptionId: subscriptionId_example,
  } satisfies DeleteEventSubscriptionRequest;

  try {
    const data = await api.deleteEventSubscription(body);
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
| **subscriptionId** | `string` |  | [Defaults to `undefined`] |

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


## listEventSubscriptions

> Array&lt;EventSubscription&gt; listEventSubscriptions()



### Example

```ts
import {
  Configuration,
  EventSubscriptionApi,
} from '@simplebilly/api';
import type { ListEventSubscriptionsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventSubscriptionApi(config);

  try {
    const data = await api.listEventSubscriptions();
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

[**Array&lt;EventSubscription&gt;**](EventSubscription.md)

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

