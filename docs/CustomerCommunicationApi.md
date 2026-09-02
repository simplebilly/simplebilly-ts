# CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCommunication**](CustomerCommunicationApi.md#createcommunication) | **POST** /api/v1/communications |  |
| [**customercommunicationRestore**](CustomerCommunicationApi.md#customercommunicationrestore) | **POST** /api/v1/communications/{communication_id}/restore |  |
| [**deleteCommunication**](CustomerCommunicationApi.md#deletecommunication) | **DELETE** /api/v1/communications/{communication_id} |  |
| [**getCommunication**](CustomerCommunicationApi.md#getcommunication) | **GET** /api/v1/communications/{communication_id} |  |
| [**getContactHistory**](CustomerCommunicationApi.md#getcontacthistory) | **GET** /api/v1/contacts/{contact_id}/communications |  |
| [**listCommunications**](CustomerCommunicationApi.md#listcommunications) | **GET** /api/v1/communications/ |  |
| [**updateCommunication**](CustomerCommunicationApi.md#updatecommunication) | **PUT** /api/v1/communications/{communication_id} |  |



## createCommunication

> CustomerCommunication createCommunication(customerCommunicationCreate)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { CreateCommunicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // CustomerCommunicationCreate
    customerCommunicationCreate: ...,
  } satisfies CreateCommunicationRequest;

  try {
    const data = await api.createCommunication(body);
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
| **customerCommunicationCreate** | [CustomerCommunicationCreate](CustomerCommunicationCreate.md) |  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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


## customercommunicationRestore

> CustomerCommunication customercommunicationRestore(communicationId)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { CustomercommunicationRestoreRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // string
    communicationId: communicationId_example,
  } satisfies CustomercommunicationRestoreRequest;

  try {
    const data = await api.customercommunicationRestore(body);
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
| **communicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Restored |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteCommunication

> deleteCommunication(communicationId)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { DeleteCommunicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // string
    communicationId: communicationId_example,
  } satisfies DeleteCommunicationRequest;

  try {
    const data = await api.deleteCommunication(body);
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
| **communicationId** | `string` |  | [Defaults to `undefined`] |

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


## getCommunication

> CustomerCommunication getCommunication(communicationId)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { GetCommunicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // string
    communicationId: communicationId_example,
  } satisfies GetCommunicationRequest;

  try {
    const data = await api.getCommunication(body);
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
| **communicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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


## getContactHistory

> ContactHistoryResponse getContactHistory(contactId)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { GetContactHistoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // string
    contactId: contactId_example,
  } satisfies GetContactHistoryRequest;

  try {
    const data = await api.getContactHistory(body);
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
| **contactId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ContactHistoryResponse**](ContactHistoryResponse.md)

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


## listCommunications

> Array&lt;CustomerCommunication&gt; listCommunications(page, pageSize, contactId, channel, direction, from, to)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { ListCommunicationsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string | Filter history to a single contact. (optional)
    contactId: contactId_example,
    // CommunicationChannel (optional)
    channel: ...,
    // CommunicationDirection (optional)
    direction: ...,
    // Date | Only include communications after this ISO date (inclusive). (optional)
    from: 2013-10-20,
    // Date | Only include communications before this ISO date (inclusive). (optional)
    to: 2013-10-20,
  } satisfies ListCommunicationsRequest;

  try {
    const data = await api.listCommunications(body);
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
| **contactId** | `string` | Filter history to a single contact. | [Optional] [Defaults to `undefined`] |
| **channel** | `CommunicationChannel` |  | [Optional] [Defaults to `undefined`] [Enum: email, call, meeting, chat, note] |
| **direction** | `CommunicationDirection` |  | [Optional] [Defaults to `undefined`] [Enum: inbound, outbound] |
| **from** | `Date` | Only include communications after this ISO date (inclusive). | [Optional] [Defaults to `undefined`] |
| **to** | `Date` | Only include communications before this ISO date (inclusive). | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;CustomerCommunication&gt;**](CustomerCommunication.md)

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


## updateCommunication

> CustomerCommunication updateCommunication(communicationId, customerCommunicationUpdate)



### Example

```ts
import {
  Configuration,
  CustomerCommunicationApi,
} from '@simplebilly/api';
import type { UpdateCommunicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerCommunicationApi(config);

  const body = {
    // string
    communicationId: communicationId_example,
    // CustomerCommunicationUpdate
    customerCommunicationUpdate: ...,
  } satisfies UpdateCommunicationRequest;

  try {
    const data = await api.updateCommunication(body);
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
| **communicationId** | `string` |  | [Defaults to `undefined`] |
| **customerCommunicationUpdate** | [CustomerCommunicationUpdate](CustomerCommunicationUpdate.md) |  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

