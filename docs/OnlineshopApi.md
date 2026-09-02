# OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getSmtpConfigApi**](OnlineshopApi.md#getsmtpconfigapi) | **GET** /api/v1/settings/smtp |  |
| [**saveSmtpConfigApi**](OnlineshopApi.md#savesmtpconfigapi) | **PUT** /api/v1/settings/smtp |  |



## getSmtpConfigApi

> SmtpConfig getSmtpConfigApi()



### Example

```ts
import {
  Configuration,
  OnlineshopApi,
} from '@simplebilly/api';
import type { GetSmtpConfigApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OnlineshopApi(config);

  try {
    const data = await api.getSmtpConfigApi();
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

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant SMTP config (null if unset) |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## saveSmtpConfigApi

> SmtpConfig saveSmtpConfigApi(smtpConfig)



### Example

```ts
import {
  Configuration,
  OnlineshopApi,
} from '@simplebilly/api';
import type { SaveSmtpConfigApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OnlineshopApi(config);

  const body = {
    // SmtpConfig (optional)
    smtpConfig: ...,
  } satisfies SaveSmtpConfigApiRequest;

  try {
    const data = await api.saveSmtpConfigApi(body);
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
| **smtpConfig** | [SmtpConfig](SmtpConfig.md) |  | [Optional] |

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant SMTP config saved |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

