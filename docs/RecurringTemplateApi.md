# RecurringTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createRecurringTemplate**](RecurringTemplateApi.md#createrecurringtemplate) | **POST** /api/v1/recurring-templates |  |
| [**deleteRecurringTemplate**](RecurringTemplateApi.md#deleterecurringtemplate) | **DELETE** /api/v1/recurring-templates/{template_id} |  |
| [**getRecurringTemplate**](RecurringTemplateApi.md#getrecurringtemplate) | **GET** /api/v1/recurring-templates/{template_id} |  |
| [**listRecurringTemplates**](RecurringTemplateApi.md#listrecurringtemplates) | **GET** /api/v1/recurring-templates/ |  |



## createRecurringTemplate

> RecurringTemplate createRecurringTemplate(body)



### Example

```ts
import {
  Configuration,
  RecurringTemplateApi,
} from '@simplebilly/api';
import type { CreateRecurringTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RecurringTemplateApi(config);

  const body = {
    // any
    body: ...,
  } satisfies CreateRecurringTemplateRequest;

  try {
    const data = await api.createRecurringTemplate(body);
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

[**RecurringTemplate**](RecurringTemplate.md)

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


## deleteRecurringTemplate

> deleteRecurringTemplate(templateId)



### Example

```ts
import {
  Configuration,
  RecurringTemplateApi,
} from '@simplebilly/api';
import type { DeleteRecurringTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RecurringTemplateApi(config);

  const body = {
    // string
    templateId: templateId_example,
  } satisfies DeleteRecurringTemplateRequest;

  try {
    const data = await api.deleteRecurringTemplate(body);
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
| **templateId** | `string` |  | [Defaults to `undefined`] |

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


## getRecurringTemplate

> RecurringTemplate getRecurringTemplate(templateId)



### Example

```ts
import {
  Configuration,
  RecurringTemplateApi,
} from '@simplebilly/api';
import type { GetRecurringTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RecurringTemplateApi(config);

  const body = {
    // string
    templateId: templateId_example,
  } satisfies GetRecurringTemplateRequest;

  try {
    const data = await api.getRecurringTemplate(body);
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
| **templateId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**RecurringTemplate**](RecurringTemplate.md)

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


## listRecurringTemplates

> Array&lt;RecurringTemplate&gt; listRecurringTemplates()



### Example

```ts
import {
  Configuration,
  RecurringTemplateApi,
} from '@simplebilly/api';
import type { ListRecurringTemplatesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RecurringTemplateApi(config);

  try {
    const data = await api.listRecurringTemplates();
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

[**Array&lt;RecurringTemplate&gt;**](RecurringTemplate.md)

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

