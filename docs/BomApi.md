# BomApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createBom**](BomApi.md#createbom) | **POST** /api/v1/boms |  |
| [**deleteBom**](BomApi.md#deletebom) | **DELETE** /api/v1/boms/{bom_id} |  |
| [**getBom**](BomApi.md#getbom) | **GET** /api/v1/boms/{bom_id} |  |
| [**listBoms**](BomApi.md#listboms) | **GET** /api/v1/boms/ |  |
| [**updateBom**](BomApi.md#updatebom) | **PUT** /api/v1/boms/{bom_id} |  |



## createBom

> Bom createBom(bomCreate)



### Example

```ts
import {
  Configuration,
  BomApi,
} from '@simplebilly/api';
import type { CreateBomRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BomApi(config);

  const body = {
    // BomCreate
    bomCreate: ...,
  } satisfies CreateBomRequest;

  try {
    const data = await api.createBom(body);
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
| **bomCreate** | [BomCreate](BomCreate.md) |  | |

### Return type

[**Bom**](Bom.md)

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


## deleteBom

> deleteBom(bomId)



### Example

```ts
import {
  Configuration,
  BomApi,
} from '@simplebilly/api';
import type { DeleteBomRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BomApi(config);

  const body = {
    // string
    bomId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteBomRequest;

  try {
    const data = await api.deleteBom(body);
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
| **bomId** | `string` |  | [Defaults to `undefined`] |

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


## getBom

> Bom getBom(bomId)



### Example

```ts
import {
  Configuration,
  BomApi,
} from '@simplebilly/api';
import type { GetBomRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BomApi(config);

  const body = {
    // string
    bomId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetBomRequest;

  try {
    const data = await api.getBom(body);
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
| **bomId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Bom**](Bom.md)

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


## listBoms

> Array&lt;Bom&gt; listBoms(page, pageSize, search, productId)



### Example

```ts
import {
  Configuration,
  BomApi,
} from '@simplebilly/api';
import type { ListBomsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BomApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // string | Filter by finished product id. (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListBomsRequest;

  try {
    const data = await api.listBoms(body);
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
| **productId** | `string` | Filter by finished product id. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Bom&gt;**](Bom.md)

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


## updateBom

> Bom updateBom(bomId, bomUpdate)



### Example

```ts
import {
  Configuration,
  BomApi,
} from '@simplebilly/api';
import type { UpdateBomRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BomApi(config);

  const body = {
    // string
    bomId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // BomUpdate
    bomUpdate: ...,
  } satisfies UpdateBomRequest;

  try {
    const data = await api.updateBom(body);
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
| **bomId** | `string` |  | [Defaults to `undefined`] |
| **bomUpdate** | [BomUpdate](BomUpdate.md) |  | |

### Return type

[**Bom**](Bom.md)

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

