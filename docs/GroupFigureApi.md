# GroupFigureApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createGroupFigure**](GroupFigureApi.md#creategroupfigure) | **POST** /api/v1/group-figures |  |
| [**deleteGroupFigure**](GroupFigureApi.md#deletegroupfigure) | **DELETE** /api/v1/group-figures/{year} |  |
| [**getGroupFigure**](GroupFigureApi.md#getgroupfigure) | **GET** /api/v1/group-figures/{year} |  |
| [**getGroupFigures**](GroupFigureApi.md#getgroupfigures) | **GET** /api/v1/group-figures/ |  |
| [**updateGroupFigure**](GroupFigureApi.md#updategroupfigure) | **PUT** /api/v1/group-figures/{year} |  |



## createGroupFigure

> GroupFigure createGroupFigure(groupFigureCreate)



### Example

```ts
import {
  Configuration,
  GroupFigureApi,
} from '@simplebilly/api';
import type { CreateGroupFigureRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GroupFigureApi(config);

  const body = {
    // GroupFigureCreate
    groupFigureCreate: ...,
  } satisfies CreateGroupFigureRequest;

  try {
    const data = await api.createGroupFigure(body);
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
| **groupFigureCreate** | [GroupFigureCreate](GroupFigureCreate.md) |  | |

### Return type

[**GroupFigure**](GroupFigure.md)

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


## deleteGroupFigure

> deleteGroupFigure(year)



### Example

```ts
import {
  Configuration,
  GroupFigureApi,
} from '@simplebilly/api';
import type { DeleteGroupFigureRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GroupFigureApi(config);

  const body = {
    // number
    year: 56,
  } satisfies DeleteGroupFigureRequest;

  try {
    const data = await api.deleteGroupFigure(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

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


## getGroupFigure

> GroupFigure getGroupFigure(year)



### Example

```ts
import {
  Configuration,
  GroupFigureApi,
} from '@simplebilly/api';
import type { GetGroupFigureRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GroupFigureApi(config);

  const body = {
    // number
    year: 56,
  } satisfies GetGroupFigureRequest;

  try {
    const data = await api.getGroupFigure(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**GroupFigure**](GroupFigure.md)

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


## getGroupFigures

> Array&lt;GroupFigure&gt; getGroupFigures(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  GroupFigureApi,
} from '@simplebilly/api';
import type { GetGroupFiguresRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GroupFigureApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies GetGroupFiguresRequest;

  try {
    const data = await api.getGroupFigures(body);
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

[**Array&lt;GroupFigure&gt;**](GroupFigure.md)

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


## updateGroupFigure

> GroupFigure updateGroupFigure(year, groupFigureUpdate)



### Example

```ts
import {
  Configuration,
  GroupFigureApi,
} from '@simplebilly/api';
import type { UpdateGroupFigureRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GroupFigureApi(config);

  const body = {
    // number
    year: 56,
    // GroupFigureUpdate
    groupFigureUpdate: ...,
  } satisfies UpdateGroupFigureRequest;

  try {
    const data = await api.updateGroupFigure(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |
| **groupFigureUpdate** | [GroupFigureUpdate](GroupFigureUpdate.md) |  | |

### Return type

[**GroupFigure**](GroupFigure.md)

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

