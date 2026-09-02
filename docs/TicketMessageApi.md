# TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listMessagesApi**](TicketMessageApi.md#listmessagesapi) | **GET** /api/v1/support/tickets/{ticket_id}/messages |  |
| [**sendMessageApi**](TicketMessageApi.md#sendmessageapi) | **POST** /api/v1/support/tickets/{ticket_id}/messages |  |



## listMessagesApi

> Array&lt;TicketMessage&gt; listMessagesApi(ticketId)



### Example

```ts
import {
  Configuration,
  TicketMessageApi,
} from '@simplebilly/api';
import type { ListMessagesApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TicketMessageApi(config);

  const body = {
    // string
    ticketId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListMessagesApiRequest;

  try {
    const data = await api.listMessagesApi(body);
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

[**Array&lt;TicketMessage&gt;**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Messages for a ticket |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendMessageApi

> TicketMessage sendMessageApi(ticketId, sendMessageDto)



### Example

```ts
import {
  Configuration,
  TicketMessageApi,
} from '@simplebilly/api';
import type { SendMessageApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TicketMessageApi(config);

  const body = {
    // string
    ticketId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // SendMessageDto
    sendMessageDto: ...,
  } satisfies SendMessageApiRequest;

  try {
    const data = await api.sendMessageApi(body);
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
| **sendMessageDto** | [SendMessageDto](SendMessageDto.md) |  | |

### Return type

[**TicketMessage**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Message sent |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

