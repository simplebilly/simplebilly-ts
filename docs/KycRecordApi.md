# KycRecordApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createKycRecord**](KycRecordApi.md#createkycrecord) | **POST** /api/v1/kyc-records |  |
| [**deleteKycRecord**](KycRecordApi.md#deletekycrecord) | **DELETE** /api/v1/kyc-records/{id} |  |
| [**getKycRecord**](KycRecordApi.md#getkycrecord) | **GET** /api/v1/kyc-records/{id} |  |
| [**getKycRecords**](KycRecordApi.md#getkycrecords) | **GET** /api/v1/kyc-records/ |  |
| [**updateKycRecord**](KycRecordApi.md#updatekycrecord) | **PUT** /api/v1/kyc-records/{id} |  |



## createKycRecord

> KycRecord createKycRecord(kycRecordCreate)



### Example

```ts
import {
  Configuration,
  KycRecordApi,
} from '@simplebilly/api';
import type { CreateKycRecordRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KycRecordApi(config);

  const body = {
    // KycRecordCreate
    kycRecordCreate: ...,
  } satisfies CreateKycRecordRequest;

  try {
    const data = await api.createKycRecord(body);
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
| **kycRecordCreate** | [KycRecordCreate](KycRecordCreate.md) |  | |

### Return type

[**KycRecord**](KycRecord.md)

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


## deleteKycRecord

> deleteKycRecord(id)



### Example

```ts
import {
  Configuration,
  KycRecordApi,
} from '@simplebilly/api';
import type { DeleteKycRecordRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KycRecordApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteKycRecordRequest;

  try {
    const data = await api.deleteKycRecord(body);
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


## getKycRecord

> KycRecord getKycRecord(id)



### Example

```ts
import {
  Configuration,
  KycRecordApi,
} from '@simplebilly/api';
import type { GetKycRecordRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KycRecordApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetKycRecordRequest;

  try {
    const data = await api.getKycRecord(body);
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

[**KycRecord**](KycRecord.md)

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


## getKycRecords

> Array&lt;KycRecord&gt; getKycRecords(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  KycRecordApi,
} from '@simplebilly/api';
import type { GetKycRecordsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KycRecordApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetKycRecordsRequest;

  try {
    const data = await api.getKycRecords(body);
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

[**Array&lt;KycRecord&gt;**](KycRecord.md)

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


## updateKycRecord

> KycRecord updateKycRecord(id, kycRecordUpdate)



### Example

```ts
import {
  Configuration,
  KycRecordApi,
} from '@simplebilly/api';
import type { UpdateKycRecordRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KycRecordApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // KycRecordUpdate
    kycRecordUpdate: ...,
  } satisfies UpdateKycRecordRequest;

  try {
    const data = await api.updateKycRecord(body);
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
| **kycRecordUpdate** | [KycRecordUpdate](KycRecordUpdate.md) |  | |

### Return type

[**KycRecord**](KycRecord.md)

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

