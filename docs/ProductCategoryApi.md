# ProductCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProductCategory**](ProductCategoryApi.md#createproductcategory) | **POST** /api/v1/product-categories |  |
| [**deleteProductCategory**](ProductCategoryApi.md#deleteproductcategory) | **DELETE** /api/v1/product-categories/{category_id} |  |
| [**getProductCategory**](ProductCategoryApi.md#getproductcategory) | **GET** /api/v1/product-categories/{category_id} |  |
| [**listProductCategories**](ProductCategoryApi.md#listproductcategories) | **GET** /api/v1/product-categories |  |
| [**updateProductCategory**](ProductCategoryApi.md#updateproductcategory) | **PUT** /api/v1/product-categories/{category_id} |  |



## createProductCategory

> ProductCategory createProductCategory(productCategory)



### Example

```ts
import {
  Configuration,
  ProductCategoryApi,
} from '@simplebilly/api';
import type { CreateProductCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductCategoryApi(config);

  const body = {
    // ProductCategory
    productCategory: ...,
  } satisfies CreateProductCategoryRequest;

  try {
    const data = await api.createProductCategory(body);
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
| **productCategory** | [ProductCategory](ProductCategory.md) |  | |

### Return type

[**ProductCategory**](ProductCategory.md)

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


## deleteProductCategory

> deleteProductCategory(categoryId)



### Example

```ts
import {
  Configuration,
  ProductCategoryApi,
} from '@simplebilly/api';
import type { DeleteProductCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductCategoryApi(config);

  const body = {
    // string
    categoryId: categoryId_example,
  } satisfies DeleteProductCategoryRequest;

  try {
    const data = await api.deleteProductCategory(body);
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
| **categoryId** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Deleted |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getProductCategory

> ProductCategory getProductCategory(categoryId)



### Example

```ts
import {
  Configuration,
  ProductCategoryApi,
} from '@simplebilly/api';
import type { GetProductCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductCategoryApi(config);

  const body = {
    // string
    categoryId: categoryId_example,
  } satisfies GetProductCategoryRequest;

  try {
    const data = await api.getProductCategory(body);
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
| **categoryId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProductCategory**](ProductCategory.md)

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


## listProductCategories

> Array&lt;ProductCategory&gt; listProductCategories()



### Example

```ts
import {
  Configuration,
  ProductCategoryApi,
} from '@simplebilly/api';
import type { ListProductCategoriesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductCategoryApi(config);

  try {
    const data = await api.listProductCategories();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;ProductCategory&gt;**](ProductCategory.md)

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


## updateProductCategory

> ProductCategory updateProductCategory(categoryId, body)



### Example

```ts
import {
  Configuration,
  ProductCategoryApi,
} from '@simplebilly/api';
import type { UpdateProductCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductCategoryApi(config);

  const body = {
    // string
    categoryId: categoryId_example,
    // any
    body: ...,
  } satisfies UpdateProductCategoryRequest;

  try {
    const data = await api.updateProductCategory(body);
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
| **categoryId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**ProductCategory**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

