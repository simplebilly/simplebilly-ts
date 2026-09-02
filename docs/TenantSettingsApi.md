# TenantSettingsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getTenantSettings**](TenantSettingsApi.md#gettenantsettings) | **GET** /api/v1/settings/tenant |  |
| [**updateTenantSettings**](TenantSettingsApi.md#updatetenantsettings) | **PUT** /api/v1/settings/tenant |  |



## getTenantSettings

> TenantSettings getTenantSettings()



### Example

```ts
import {
  Configuration,
  TenantSettingsApi,
} from '@simplebilly/api';
import type { GetTenantSettingsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TenantSettingsApi(config);

  try {
    const data = await api.getTenantSettings();
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

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant settings |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTenantSettings

> TenantSettings updateTenantSettings(updateTenantSettings)



### Example

```ts
import {
  Configuration,
  TenantSettingsApi,
} from '@simplebilly/api';
import type { UpdateTenantSettingsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TenantSettingsApi(config);

  const body = {
    // UpdateTenantSettings
    updateTenantSettings: ...,
  } satisfies UpdateTenantSettingsRequest;

  try {
    const data = await api.updateTenantSettings(body);
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
| **updateTenantSettings** | [UpdateTenantSettings](UpdateTenantSettings.md) |  | |

### Return type

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated tenant settings |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

