# SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTicketApi**](SupportTicketApi.md#createticketapi) | **POST** /api/v1/support/tickets |  |
| [**deleteTicketApi**](SupportTicketApi.md#deleteticketapi) | **DELETE** /api/v1/support/tickets/{ticket_id} |  |
| [**getTicketApi**](SupportTicketApi.md#getticketapi) | **GET** /api/v1/support/tickets/{ticket_id} |  |
| [**listTicketsApi**](SupportTicketApi.md#listticketsapi) | **GET** /api/v1/support/tickets |  |
| [**updateTicketApi**](SupportTicketApi.md#updateticketapi) | **PUT** /api/v1/support/tickets/{ticket_id} |  |



## createTicketApi

> SupportTicket createTicketApi(createTicketRequest)



### Example

```ts
import {
  Configuration,
  SupportTicketApi,
} from '@simplebilly/api';
import type { CreateTicketApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportTicketApi(config);

  const body = {
    // CreateTicketRequest
    createTicketRequest: ...,
  } satisfies CreateTicketApiRequest;

  try {
    const data = await api.createTicketApi(body);
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
| **createTicketRequest** | [CreateTicketRequest](CreateTicketRequest.md) |  | |

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Ticket created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTicketApi

> deleteTicketApi(ticketId)



### Example

```ts
import {
  Configuration,
  SupportTicketApi,
} from '@simplebilly/api';
import type { DeleteTicketApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportTicketApi(config);

  const body = {
    // string
    ticketId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteTicketApiRequest;

  try {
    const data = await api.deleteTicketApi(body);
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
| **ticketId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Ticket deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTicketApi

> SupportTicket getTicketApi(ticketId)



### Example

```ts
import {
  Configuration,
  SupportTicketApi,
} from '@simplebilly/api';
import type { GetTicketApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportTicketApi(config);

  const body = {
    // string
    ticketId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetTicketApiRequest;

  try {
    const data = await api.getTicketApi(body);
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
| **ticketId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ticket detail |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTicketsApi

> Array&lt;SupportTicket&gt; listTicketsApi(status, priority, assignedTo, channelType, customerId, search, page, pageSize)



### Example

```ts
import {
  Configuration,
  SupportTicketApi,
} from '@simplebilly/api';
import type { ListTicketsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportTicketApi(config);

  const body = {
    // string (optional)
    status: status_example,
    // string (optional)
    priority: priority_example,
    // string (optional)
    assignedTo: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    channelType: channelType_example,
    // string (optional)
    customerId: customerId_example,
    // string (optional)
    search: search_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies ListTicketsApiRequest;

  try {
    const data = await api.listTicketsApi(body);
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
| **priority** | `string` |  | [Optional] [Defaults to `undefined`] |
| **assignedTo** | `string` |  | [Optional] [Defaults to `undefined`] |
| **channelType** | `string` |  | [Optional] [Defaults to `undefined`] |
| **customerId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;SupportTicket&gt;**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tickets list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTicketApi

> SupportTicket updateTicketApi(ticketId, supportTicketUpdate)



### Example

```ts
import {
  Configuration,
  SupportTicketApi,
} from '@simplebilly/api';
import type { UpdateTicketApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportTicketApi(config);

  const body = {
    // string
    ticketId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // SupportTicketUpdate
    supportTicketUpdate: ...,
  } satisfies UpdateTicketApiRequest;

  try {
    const data = await api.updateTicketApi(body);
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
| **ticketId** | `string` |  | [Defaults to `undefined`] |
| **supportTicketUpdate** | [SupportTicketUpdate](SupportTicketUpdate.md) |  | |

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ticket updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

