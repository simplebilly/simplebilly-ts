# CustomerGroupApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addGroupMembers**](CustomerGroupApi.md#addgroupmembers) | **POST** /api/v1/customer-groups/{customer_group_id}/members |  |
| [**createCustomerGroup**](CustomerGroupApi.md#createcustomergroup) | **POST** /api/v1/customer-groups |  |
| [**deleteCustomerGroup**](CustomerGroupApi.md#deletecustomergroup) | **DELETE** /api/v1/customer-groups/{customer_group_id} |  |
| [**getCustomerGroup**](CustomerGroupApi.md#getcustomergroup) | **GET** /api/v1/customer-groups/{customer_group_id} |  |
| [**listCustomerGroups**](CustomerGroupApi.md#listcustomergroups) | **GET** /api/v1/customer-groups/ |  |
| [**updateCustomerGroup**](CustomerGroupApi.md#updatecustomergroup) | **PUT** /api/v1/customer-groups/{customer_group_id} |  |



## addGroupMembers

> CustomerGroup addGroupMembers(customerGroupId, body)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { AddGroupMembersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // string
    customerGroupId: customerGroupId_example,
    // any
    body: ...,
  } satisfies AddGroupMembersRequest;

  try {
    const data = await api.addGroupMembers(body);
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
| **customerGroupId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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


## createCustomerGroup

> CustomerGroup createCustomerGroup(customerGroupCreate)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { CreateCustomerGroupRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // CustomerGroupCreate
    customerGroupCreate: ...,
  } satisfies CreateCustomerGroupRequest;

  try {
    const data = await api.createCustomerGroup(body);
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
| **customerGroupCreate** | [CustomerGroupCreate](CustomerGroupCreate.md) |  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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


## deleteCustomerGroup

> deleteCustomerGroup(customerGroupId)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { DeleteCustomerGroupRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // string
    customerGroupId: customerGroupId_example,
  } satisfies DeleteCustomerGroupRequest;

  try {
    const data = await api.deleteCustomerGroup(body);
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
| **customerGroupId** | `string` |  | [Defaults to `undefined`] |

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


## getCustomerGroup

> CustomerGroup getCustomerGroup(customerGroupId)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { GetCustomerGroupRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // string
    customerGroupId: customerGroupId_example,
  } satisfies GetCustomerGroupRequest;

  try {
    const data = await api.getCustomerGroup(body);
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
| **customerGroupId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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


## listCustomerGroups

> Array&lt;CustomerGroup&gt; listCustomerGroups(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { ListCustomerGroupsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies ListCustomerGroupsRequest;

  try {
    const data = await api.listCustomerGroups(body);
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

[**Array&lt;CustomerGroup&gt;**](CustomerGroup.md)

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


## updateCustomerGroup

> CustomerGroup updateCustomerGroup(customerGroupId, customerGroupUpdate)



### Example

```ts
import {
  Configuration,
  CustomerGroupApi,
} from '@simplebilly/api';
import type { UpdateCustomerGroupRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomerGroupApi(config);

  const body = {
    // string
    customerGroupId: customerGroupId_example,
    // CustomerGroupUpdate
    customerGroupUpdate: ...,
  } satisfies UpdateCustomerGroupRequest;

  try {
    const data = await api.updateCustomerGroup(body);
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
| **customerGroupId** | `string` |  | [Defaults to `undefined`] |
| **customerGroupUpdate** | [CustomerGroupUpdate](CustomerGroupUpdate.md) |  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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

