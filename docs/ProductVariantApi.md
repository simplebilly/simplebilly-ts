# ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProductVariant**](ProductVariantApi.md#createproductvariant) | **POST** /api/v1/product-variants |  |
| [**deleteProductVariant**](ProductVariantApi.md#deleteproductvariant) | **DELETE** /api/v1/product-variants/{variant_id} |  |
| [**generateProductVariants**](ProductVariantApi.md#generateproductvariants) | **POST** /api/v1/product-variants/generate |  |
| [**getProductVariant**](ProductVariantApi.md#getproductvariant) | **GET** /api/v1/product-variants/{variant_id} |  |
| [**listProductVariants**](ProductVariantApi.md#listproductvariants) | **GET** /api/v1/product-variants/ |  |
| [**updateProductVariant**](ProductVariantApi.md#updateproductvariant) | **PUT** /api/v1/product-variants/{variant_id} |  |



## createProductVariant

> ProductVariant createProductVariant(productVariant)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { CreateProductVariantRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // ProductVariant
    productVariant: ...,
  } satisfies CreateProductVariantRequest;

  try {
    const data = await api.createProductVariant(body);
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
| **productVariant** | [ProductVariant](ProductVariant.md) |  | |

### Return type

[**ProductVariant**](ProductVariant.md)

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


## deleteProductVariant

> deleteProductVariant(variantId)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { DeleteProductVariantRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // string
    variantId: variantId_example,
  } satisfies DeleteProductVariantRequest;

  try {
    const data = await api.deleteProductVariant(body);
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
| **variantId** | `string` |  | [Defaults to `undefined`] |

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


## generateProductVariants

> Array&lt;ProductVariant&gt; generateProductVariants(generateVariantsRequest)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { GenerateProductVariantsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // GenerateVariantsRequest
    generateVariantsRequest: ...,
  } satisfies GenerateProductVariantsRequest;

  try {
    const data = await api.generateProductVariants(body);
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
| **generateVariantsRequest** | [GenerateVariantsRequest](GenerateVariantsRequest.md) |  | |

### Return type

[**Array&lt;ProductVariant&gt;**](ProductVariant.md)

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


## getProductVariant

> ProductVariant getProductVariant(variantId)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { GetProductVariantRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // string
    variantId: variantId_example,
  } satisfies GetProductVariantRequest;

  try {
    const data = await api.getProductVariant(body);
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
| **variantId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ProductVariant**](ProductVariant.md)

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


## listProductVariants

> Array&lt;ProductVariant&gt; listProductVariants(page, pageSize, productId, isActive)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { ListProductVariantsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // boolean (optional)
    isActive: true,
  } satisfies ListProductVariantsRequest;

  try {
    const data = await api.listProductVariants(body);
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
| **isActive** | `boolean` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ProductVariant&gt;**](ProductVariant.md)

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


## updateProductVariant

> ProductVariant updateProductVariant(variantId, body)



### Example

```ts
import {
  Configuration,
  ProductVariantApi,
} from '@simplebilly/api';
import type { UpdateProductVariantRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductVariantApi(config);

  const body = {
    // string
    variantId: variantId_example,
    // any
    body: ...,
  } satisfies UpdateProductVariantRequest;

  try {
    const data = await api.updateProductVariant(body);
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
| **variantId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

