# AutomationsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listAutomations**](AutomationsApi.md#listautomations) | **GET** /api/v1/automations |  |
| [**triggerAutomation**](AutomationsApi.md#triggerautomation) | **POST** /api/v1/automations/{key}/trigger |  |
| [**updateAutomation**](AutomationsApi.md#updateautomation) | **PUT** /api/v1/automations/{key} |  |



## listAutomations

> Array&lt;AutomationDto&gt; listAutomations()



### Example

```ts
import {
  Configuration,
  AutomationsApi,
} from '@simplebilly/api';
import type { ListAutomationsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AutomationsApi(config);

  try {
    const data = await api.listAutomations();
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

[**Array&lt;AutomationDto&gt;**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## triggerAutomation

> object triggerAutomation(key)



### Example

```ts
import {
  Configuration,
  AutomationsApi,
} from '@simplebilly/api';
import type { TriggerAutomationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AutomationsApi(config);

  const body = {
    // string
    key: key_example,
  } satisfies TriggerAutomationRequest;

  try {
    const data = await api.triggerAutomation(body);
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
| **key** | `string` |  | [Defaults to `undefined`] |

### Return type

**object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateAutomation

> AutomationDto updateAutomation(key, updateAutomation)



### Example

```ts
import {
  Configuration,
  AutomationsApi,
} from '@simplebilly/api';
import type { UpdateAutomationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AutomationsApi(config);

  const body = {
    // string
    key: key_example,
    // UpdateAutomation
    updateAutomation: ...,
  } satisfies UpdateAutomationRequest;

  try {
    const data = await api.updateAutomation(body);
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
| **key** | `string` |  | [Defaults to `undefined`] |
| **updateAutomation** | [UpdateAutomation](UpdateAutomation.md) |  | |

### Return type

[**AutomationDto**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

