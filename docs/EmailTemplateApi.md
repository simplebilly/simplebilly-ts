# EmailTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEmailTemplate**](EmailTemplateApi.md#createemailtemplate) | **POST** /api/v1/email-templates |  |
| [**deleteEmailTemplate**](EmailTemplateApi.md#deleteemailtemplate) | **DELETE** /api/v1/email-templates/{email_template_id} |  |
| [**getEmailTemplate**](EmailTemplateApi.md#getemailtemplate) | **GET** /api/v1/email-templates/{email_template_id} |  |
| [**listEmailTemplates**](EmailTemplateApi.md#listemailtemplates) | **GET** /api/v1/email-templates/ |  |
| [**renderEmailTemplate**](EmailTemplateApi.md#renderemailtemplate) | **POST** /api/v1/email-templates/{email_template_id}/render |  |
| [**updateEmailTemplate**](EmailTemplateApi.md#updateemailtemplate) | **PUT** /api/v1/email-templates/{email_template_id} |  |



## createEmailTemplate

> EmailTemplate createEmailTemplate(emailTemplateCreate)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { CreateEmailTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // EmailTemplateCreate
    emailTemplateCreate: ...,
  } satisfies CreateEmailTemplateRequest;

  try {
    const data = await api.createEmailTemplate(body);
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
| **emailTemplateCreate** | [EmailTemplateCreate](EmailTemplateCreate.md) |  | |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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


## deleteEmailTemplate

> deleteEmailTemplate(emailTemplateId)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { DeleteEmailTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // string
    emailTemplateId: emailTemplateId_example,
  } satisfies DeleteEmailTemplateRequest;

  try {
    const data = await api.deleteEmailTemplate(body);
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
| **emailTemplateId** | `string` |  | [Defaults to `undefined`] |

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


## getEmailTemplate

> EmailTemplate getEmailTemplate(emailTemplateId)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { GetEmailTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // string
    emailTemplateId: emailTemplateId_example,
  } satisfies GetEmailTemplateRequest;

  try {
    const data = await api.getEmailTemplate(body);
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
| **emailTemplateId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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


## listEmailTemplates

> Array&lt;EmailTemplate&gt; listEmailTemplates(page, pageSize, status, search)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { ListEmailTemplatesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    search: search_example,
  } satisfies ListEmailTemplatesRequest;

  try {
    const data = await api.listEmailTemplates(body);
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
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;EmailTemplate&gt;**](EmailTemplate.md)

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


## renderEmailTemplate

> any renderEmailTemplate(emailTemplateId, body)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { RenderEmailTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // string
    emailTemplateId: emailTemplateId_example,
    // any
    body: ...,
  } satisfies RenderEmailTemplateRequest;

  try {
    const data = await api.renderEmailTemplate(body);
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
| **emailTemplateId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

**any**

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


## updateEmailTemplate

> EmailTemplate updateEmailTemplate(emailTemplateId, emailTemplateUpdate)



### Example

```ts
import {
  Configuration,
  EmailTemplateApi,
} from '@simplebilly/api';
import type { UpdateEmailTemplateRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailTemplateApi(config);

  const body = {
    // string
    emailTemplateId: emailTemplateId_example,
    // EmailTemplateUpdate
    emailTemplateUpdate: ...,
  } satisfies UpdateEmailTemplateRequest;

  try {
    const data = await api.updateEmailTemplate(body);
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
| **emailTemplateId** | `string` |  | [Defaults to `undefined`] |
| **emailTemplateUpdate** | [EmailTemplateUpdate](EmailTemplateUpdate.md) |  | |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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

