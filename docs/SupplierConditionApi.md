# SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSupplierCondition**](SupplierConditionApi.md#createsuppliercondition) | **POST** /api/v1/supplier-conditions |  |
| [**deleteSupplierCondition**](SupplierConditionApi.md#deletesuppliercondition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} |  |
| [**getSupplierCondition**](SupplierConditionApi.md#getsuppliercondition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} |  |
| [**listSupplierConditions**](SupplierConditionApi.md#listsupplierconditions) | **GET** /api/v1/supplier-conditions/ |  |
| [**updateSupplierCondition**](SupplierConditionApi.md#updatesuppliercondition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} |  |



## createSupplierCondition

> SupplierCondition createSupplierCondition(supplierConditionCreate)



### Example

```ts
import {
  Configuration,
  SupplierConditionApi,
} from '@simplebilly/api';
import type { CreateSupplierConditionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierConditionApi(config);

  const body = {
    // SupplierConditionCreate
    supplierConditionCreate: ...,
  } satisfies CreateSupplierConditionRequest;

  try {
    const data = await api.createSupplierCondition(body);
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
| **supplierConditionCreate** | [SupplierConditionCreate](SupplierConditionCreate.md) |  | |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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


## deleteSupplierCondition

> deleteSupplierCondition(supplierConditionId)



### Example

```ts
import {
  Configuration,
  SupplierConditionApi,
} from '@simplebilly/api';
import type { DeleteSupplierConditionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierConditionApi(config);

  const body = {
    // string
    supplierConditionId: supplierConditionId_example,
  } satisfies DeleteSupplierConditionRequest;

  try {
    const data = await api.deleteSupplierCondition(body);
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
| **supplierConditionId** | `string` |  | [Defaults to `undefined`] |

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


## getSupplierCondition

> SupplierCondition getSupplierCondition(supplierConditionId)



### Example

```ts
import {
  Configuration,
  SupplierConditionApi,
} from '@simplebilly/api';
import type { GetSupplierConditionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierConditionApi(config);

  const body = {
    // string
    supplierConditionId: supplierConditionId_example,
  } satisfies GetSupplierConditionRequest;

  try {
    const data = await api.getSupplierCondition(body);
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
| **supplierConditionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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


## listSupplierConditions

> Array&lt;SupplierCondition&gt; listSupplierConditions(page, pageSize, supplierContactId, search)



### Example

```ts
import {
  Configuration,
  SupplierConditionApi,
} from '@simplebilly/api';
import type { ListSupplierConditionsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierConditionApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    supplierContactId: supplierContactId_example,
    // string (optional)
    search: search_example,
  } satisfies ListSupplierConditionsRequest;

  try {
    const data = await api.listSupplierConditions(body);
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
| **supplierContactId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;SupplierCondition&gt;**](SupplierCondition.md)

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


## updateSupplierCondition

> SupplierCondition updateSupplierCondition(supplierConditionId, supplierConditionUpdate)



### Example

```ts
import {
  Configuration,
  SupplierConditionApi,
} from '@simplebilly/api';
import type { UpdateSupplierConditionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupplierConditionApi(config);

  const body = {
    // string
    supplierConditionId: supplierConditionId_example,
    // SupplierConditionUpdate
    supplierConditionUpdate: ...,
  } satisfies UpdateSupplierConditionRequest;

  try {
    const data = await api.updateSupplierCondition(body);
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
| **supplierConditionId** | `string` |  | [Defaults to `undefined`] |
| **supplierConditionUpdate** | [SupplierConditionUpdate](SupplierConditionUpdate.md) |  | |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

