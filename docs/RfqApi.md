# RfqApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**convertRfq**](RfqApi.md#convertrfq) | **POST** /api/v1/rfqs/{rfq_id}/convert | Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;. |
| [**createRfq**](RfqApi.md#createrfq) | **POST** /api/v1/rfqs |  |
| [**deleteRfq**](RfqApi.md#deleterfq) | **DELETE** /api/v1/rfqs/{rfq_id} |  |
| [**getRfq**](RfqApi.md#getrfq) | **GET** /api/v1/rfqs/{rfq_id} |  |
| [**listRfqs**](RfqApi.md#listrfqs) | **GET** /api/v1/rfqs/ |  |
| [**updateRfq**](RfqApi.md#updaterfq) | **PUT** /api/v1/rfqs/{rfq_id} |  |
| [**updateRfqStatus**](RfqApi.md#updaterfqstatus) | **PUT** /api/v1/rfqs/{rfq_id}/status |  |



## convertRfq

> any convertRfq(rfqId)

Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;.

### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { ConvertRfqRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // string
    rfqId: rfqId_example,
  } satisfies ConvertRfqRequest;

  try {
    const data = await api.convertRfq(body);
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
| **rfqId** | `string` |  | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createRfq

> Rfq createRfq(rfq)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { CreateRfqRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // Rfq
    rfq: ...,
  } satisfies CreateRfqRequest;

  try {
    const data = await api.createRfq(body);
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
| **rfq** | [Rfq](Rfq.md) |  | |

### Return type

[**Rfq**](Rfq.md)

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


## deleteRfq

> deleteRfq(rfqId)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { DeleteRfqRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // string
    rfqId: rfqId_example,
  } satisfies DeleteRfqRequest;

  try {
    const data = await api.deleteRfq(body);
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
| **rfqId** | `string` |  | [Defaults to `undefined`] |

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


## getRfq

> Rfq getRfq(rfqId)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { GetRfqRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // string
    rfqId: rfqId_example,
  } satisfies GetRfqRequest;

  try {
    const data = await api.getRfq(body);
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
| **rfqId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Rfq**](Rfq.md)

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


## listRfqs

> Array&lt;Rfq&gt; listRfqs(page, pageSize, status, supplierName)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { ListRfqsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    supplierName: supplierName_example,
  } satisfies ListRfqsRequest;

  try {
    const data = await api.listRfqs(body);
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
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierName** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Rfq&gt;**](Rfq.md)

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


## updateRfq

> Rfq updateRfq(rfqId, body)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { UpdateRfqRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // string
    rfqId: rfqId_example,
    // any
    body: ...,
  } satisfies UpdateRfqRequest;

  try {
    const data = await api.updateRfq(body);
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
| **rfqId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**Rfq**](Rfq.md)

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


## updateRfqStatus

> Rfq updateRfqStatus(rfqId, rfqStatusUpdate)



### Example

```ts
import {
  Configuration,
  RfqApi,
} from '@simplebilly/api';
import type { UpdateRfqStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RfqApi(config);

  const body = {
    // string
    rfqId: rfqId_example,
    // RfqStatusUpdate
    rfqStatusUpdate: ...,
  } satisfies UpdateRfqStatusRequest;

  try {
    const data = await api.updateRfqStatus(body);
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
| **rfqId** | `string` |  | [Defaults to `undefined`] |
| **rfqStatusUpdate** | [RfqStatusUpdate](RfqStatusUpdate.md) |  | |

### Return type

[**Rfq**](Rfq.md)

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

