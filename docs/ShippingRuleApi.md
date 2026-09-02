# ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createShippingRule**](ShippingRuleApi.md#createshippingrule) | **POST** /api/v1/shipping-rules |  |
| [**deleteShippingRule**](ShippingRuleApi.md#deleteshippingrule) | **DELETE** /api/v1/shipping-rules/{rule_id} |  |
| [**getShippingRule**](ShippingRuleApi.md#getshippingrule) | **GET** /api/v1/shipping-rules/{rule_id} |  |
| [**listShippingRules**](ShippingRuleApi.md#listshippingrules) | **GET** /api/v1/shipping-rules/ |  |
| [**updateShippingRule**](ShippingRuleApi.md#updateshippingrule) | **PUT** /api/v1/shipping-rules/{rule_id} |  |



## createShippingRule

> ShippingRule createShippingRule(shippingRuleCreate)



### Example

```ts
import {
  Configuration,
  ShippingRuleApi,
} from '@simplebilly/api';
import type { CreateShippingRuleRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingRuleApi(config);

  const body = {
    // ShippingRuleCreate
    shippingRuleCreate: ...,
  } satisfies CreateShippingRuleRequest;

  try {
    const data = await api.createShippingRule(body);
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
| **shippingRuleCreate** | [ShippingRuleCreate](ShippingRuleCreate.md) |  | |

### Return type

[**ShippingRule**](ShippingRule.md)

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


## deleteShippingRule

> deleteShippingRule(ruleId)



### Example

```ts
import {
  Configuration,
  ShippingRuleApi,
} from '@simplebilly/api';
import type { DeleteShippingRuleRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingRuleApi(config);

  const body = {
    // string
    ruleId: ruleId_example,
  } satisfies DeleteShippingRuleRequest;

  try {
    const data = await api.deleteShippingRule(body);
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
| **ruleId** | `string` |  | [Defaults to `undefined`] |

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


## getShippingRule

> ShippingRule getShippingRule(ruleId)



### Example

```ts
import {
  Configuration,
  ShippingRuleApi,
} from '@simplebilly/api';
import type { GetShippingRuleRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingRuleApi(config);

  const body = {
    // string
    ruleId: ruleId_example,
  } satisfies GetShippingRuleRequest;

  try {
    const data = await api.getShippingRule(body);
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
| **ruleId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ShippingRule**](ShippingRule.md)

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


## listShippingRules

> Array&lt;ShippingRule&gt; listShippingRules(page, pageSize, country)



### Example

```ts
import {
  Configuration,
  ShippingRuleApi,
} from '@simplebilly/api';
import type { ListShippingRulesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingRuleApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    country: country_example,
  } satisfies ListShippingRulesRequest;

  try {
    const data = await api.listShippingRules(body);
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
| **country** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;ShippingRule&gt;**](ShippingRule.md)

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


## updateShippingRule

> ShippingRule updateShippingRule(ruleId, shippingRuleUpdate)



### Example

```ts
import {
  Configuration,
  ShippingRuleApi,
} from '@simplebilly/api';
import type { UpdateShippingRuleRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShippingRuleApi(config);

  const body = {
    // string
    ruleId: ruleId_example,
    // ShippingRuleUpdate
    shippingRuleUpdate: ...,
  } satisfies UpdateShippingRuleRequest;

  try {
    const data = await api.updateShippingRule(body);
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
| **ruleId** | `string` |  | [Defaults to `undefined`] |
| **shippingRuleUpdate** | [ShippingRuleUpdate](ShippingRuleUpdate.md) |  | |

### Return type

[**ShippingRule**](ShippingRule.md)

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

