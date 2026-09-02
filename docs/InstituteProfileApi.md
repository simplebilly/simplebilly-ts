# InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getInstituteProfile**](InstituteProfileApi.md#getinstituteprofile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing). |
| [**updateInstituteProfile**](InstituteProfileApi.md#updateinstituteprofile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert). |



## getInstituteProfile

> InstituteProfile getInstituteProfile()

Current institute profile (created with defaults when missing).

### Example

```ts
import {
  Configuration,
  InstituteProfileApi,
} from '@simplebilly/api';
import type { GetInstituteProfileRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InstituteProfileApi(config);

  try {
    const data = await api.getInstituteProfile();
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

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Institute profile |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateInstituteProfile

> InstituteProfile updateInstituteProfile(instituteProfileUpdate)

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Example

```ts
import {
  Configuration,
  InstituteProfileApi,
} from '@simplebilly/api';
import type { UpdateInstituteProfileRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InstituteProfileApi(config);

  const body = {
    // InstituteProfileUpdate
    instituteProfileUpdate: ...,
  } satisfies UpdateInstituteProfileRequest;

  try {
    const data = await api.updateInstituteProfile(body);
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
| **instituteProfileUpdate** | [InstituteProfileUpdate](InstituteProfileUpdate.md) |  | |

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated institute profile |  -  |
| **400** | Invalid institute_type |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

