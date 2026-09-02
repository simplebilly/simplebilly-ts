# ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProductAttribute**](ProductAttributeApi.md#createproductattribute) | **POST** /api/v1/product-attributes |  |
| [**deleteProductAttribute**](ProductAttributeApi.md#deleteproductattribute) | **DELETE** /api/v1/product-attributes/{attribute_id} |  |
| [**getProductAttribute**](ProductAttributeApi.md#getproductattribute) | **GET** /api/v1/product-attributes/{attribute_id} |  |
| [**listProductAttributes**](ProductAttributeApi.md#listproductattributes) | **GET** /api/v1/product-attributes/ |  |
| [**updateProductAttribute**](ProductAttributeApi.md#updateproductattribute) | **PUT** /api/v1/product-attributes/{attribute_id} |  |



## createProductAttribute

> ProductAttribute createProductAttribute(productAttributeCreate)



### Example

```ts
import {
  Configuration,
  ProductAttributeApi,
} from '@simplebilly/api';
import type { CreateProductAttributeRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductAttributeApi(config);

  const body = {
    // ProductAttributeCreate
    productAttributeCreate: ...,
  } satisfies CreateProductAttributeRequest;

  try {
    const data = await api.createProductAttribute(body);
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
| **productAttributeCreate** | [ProductAttributeCreate](ProductAttributeCreate.md) |  | |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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


## deleteProductAttribute

> deleteProductAttribute(attributeId)



### Example

```ts
import {
  Configuration,
  ProductAttributeApi,
} from '@simplebilly/api';
import type { DeleteProductAttributeRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductAttributeApi(config);

  const body = {
    // string
    attributeId: attributeId_example,
  } satisfies DeleteProductAttributeRequest;

  try {
    const data = await api.deleteProductAttribute(body);
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
| **attributeId** | `string` |  | [Defaults to `undefined`] |

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


## getProductAttribute

> ProductAttribute getProductAttribute(attributeId)



### Example

```ts
import {
  Configuration,
  ProductAttributeApi,
} from '@simplebilly/api';
import type { GetProductAttributeRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductAttributeApi(config);

  const body = {
    // string
    attributeId: attributeId_example,
  } satisfies GetProductAttributeRequest;

  try {
    const data = await api.getProductAttribute(body);
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
| **attributeId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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


## listProductAttributes

> Array&lt;ProductAttribute&gt; listProductAttributes(page, pageSize, productId, isFilterable, search)



### Example

```ts
import {
  Configuration,
  ProductAttributeApi,
} from '@simplebilly/api';
import type { ListProductAttributesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductAttributeApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // boolean (optional)
    isFilterable: true,
    // string (optional)
    search: search_example,
  } satisfies ListProductAttributesRequest;

  try {
    const data = await api.listProductAttributes(body);
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
| **productId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **isFilterable** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProductAttribute&gt;**](ProductAttribute.md)

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


## updateProductAttribute

> ProductAttribute updateProductAttribute(attributeId, productAttributeUpdate)



### Example

```ts
import {
  Configuration,
  ProductAttributeApi,
} from '@simplebilly/api';
import type { UpdateProductAttributeRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductAttributeApi(config);

  const body = {
    // string
    attributeId: attributeId_example,
    // ProductAttributeUpdate
    productAttributeUpdate: ...,
  } satisfies UpdateProductAttributeRequest;

  try {
    const data = await api.updateProductAttribute(body);
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
| **attributeId** | `string` |  | [Defaults to `undefined`] |
| **productAttributeUpdate** | [ProductAttributeUpdate](ProductAttributeUpdate.md) |  | |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

