# PostingCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPostingCategory**](PostingCategoryApi.md#createpostingcategory) | **POST** /api/v1/posting-categories |  |
| [**deletePostingCategory**](PostingCategoryApi.md#deletepostingcategory) | **DELETE** /api/v1/posting-categories/{category_id} |  |
| [**listPostingCategories**](PostingCategoryApi.md#listpostingcategories) | **GET** /api/v1/posting-categories |  |
| [**seedPostingCategories**](PostingCategoryApi.md#seedpostingcategories) | **POST** /api/v1/posting-categories/seed/{skr_version} |  |
| [**updatePostingCategory**](PostingCategoryApi.md#updatepostingcategory) | **PUT** /api/v1/posting-categories/{category_id} |  |



## createPostingCategory

> PostingCategory createPostingCategory(body)



### Example

```ts
import {
  Configuration,
  PostingCategoryApi,
} from '@simplebilly/api';
import type { CreatePostingCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PostingCategoryApi(config);

  const body = {
    // any
    body: ...,
  } satisfies CreatePostingCategoryRequest;

  try {
    const data = await api.createPostingCategory(body);
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
| **body** | `any` |  | |

### Return type

[**PostingCategory**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deletePostingCategory

> deletePostingCategory(categoryId)



### Example

```ts
import {
  Configuration,
  PostingCategoryApi,
} from '@simplebilly/api';
import type { DeletePostingCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PostingCategoryApi(config);

  const body = {
    // string
    categoryId: categoryId_example,
  } satisfies DeletePostingCategoryRequest;

  try {
    const data = await api.deletePostingCategory(body);
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


## listPostingCategories

> Array&lt;PostingCategory&gt; listPostingCategories()



### Example

```ts
import {
  Configuration,
  PostingCategoryApi,
} from '@simplebilly/api';
import type { ListPostingCategoriesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PostingCategoryApi(config);

  try {
    const data = await api.listPostingCategories();
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

[**Array&lt;PostingCategory&gt;**](PostingCategory.md)

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


## seedPostingCategories

> seedPostingCategories(skrVersion)



### Example

```ts
import {
  Configuration,
  PostingCategoryApi,
} from '@simplebilly/api';
import type { SeedPostingCategoriesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PostingCategoryApi(config);

  const body = {
    // string
    skrVersion: skrVersion_example,
  } satisfies SeedPostingCategoriesRequest;

  try {
    const data = await api.seedPostingCategories(body);
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
| **skrVersion** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Seeded |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updatePostingCategory

> PostingCategory updatePostingCategory(categoryId, body)



### Example

```ts
import {
  Configuration,
  PostingCategoryApi,
} from '@simplebilly/api';
import type { UpdatePostingCategoryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PostingCategoryApi(config);

  const body = {
    // string
    categoryId: categoryId_example,
    // any
    body: ...,
  } satisfies UpdatePostingCategoryRequest;

  try {
    const data = await api.updatePostingCategory(body);
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

[**PostingCategory**](PostingCategory.md)

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

