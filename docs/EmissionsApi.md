# EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEmissionEntryApi**](EmissionsApi.md#createemissionentryapi) | **POST** /api/v1/bookkeeping/emissions/entries |  |
| [**createEmissionTargetApi**](EmissionsApi.md#createemissiontargetapi) | **POST** /api/v1/bookkeeping/emissions/targets |  |
| [**deleteEmissionEntryApi**](EmissionsApi.md#deleteemissionentryapi) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} |  |
| [**deleteEmissionTargetApi**](EmissionsApi.md#deleteemissiontargetapi) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} |  |
| [**emissionsEntriesApi**](EmissionsApi.md#emissionsentriesapi) | **GET** /api/v1/bookkeeping/emissions/entries |  |
| [**emissionsExportApi**](EmissionsApi.md#emissionsexportapi) | **GET** /api/v1/bookkeeping/emissions/export |  |
| [**emissionsFactorsApi**](EmissionsApi.md#emissionsfactorsapi) | **GET** /api/v1/bookkeeping/emissions/factors |  |
| [**emissionsReportApi**](EmissionsApi.md#emissionsreportapi) | **GET** /api/v1/bookkeeping/emissions/report |  |
| [**emissionsTargetsApi**](EmissionsApi.md#emissionstargetsapi) | **GET** /api/v1/bookkeeping/emissions/targets |  |



## createEmissionEntryApi

> EmissionEntry createEmissionEntryApi(createEmissionEntry)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { CreateEmissionEntryApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // CreateEmissionEntry
    createEmissionEntry: ...,
  } satisfies CreateEmissionEntryApiRequest;

  try {
    const data = await api.createEmissionEntryApi(body);
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
| **createEmissionEntry** | [CreateEmissionEntry](CreateEmissionEntry.md) |  | |

### Return type

[**EmissionEntry**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Emission entry created |  -  |
| **400** | Unknown category/method |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createEmissionTargetApi

> EmissionTarget createEmissionTargetApi(createEmissionTarget)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { CreateEmissionTargetApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // CreateEmissionTarget
    createEmissionTarget: ...,
  } satisfies CreateEmissionTargetApiRequest;

  try {
    const data = await api.createEmissionTargetApi(body);
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
| **createEmissionTarget** | [CreateEmissionTarget](CreateEmissionTarget.md) |  | |

### Return type

[**EmissionTarget**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Emission target created |  -  |
| **400** | Invalid scope |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteEmissionEntryApi

> deleteEmissionEntryApi(id)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { DeleteEmissionEntryApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteEmissionEntryApiRequest;

  try {
    const data = await api.deleteEmissionEntryApi(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Emission entry deleted |  -  |
| **404** | Entry not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteEmissionTargetApi

> deleteEmissionTargetApi(id)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { DeleteEmissionTargetApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteEmissionTargetApiRequest;

  try {
    const data = await api.deleteEmissionTargetApi(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Emission target deleted |  -  |
| **404** | Target not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## emissionsEntriesApi

> Array&lt;EmissionEntry&gt; emissionsEntriesApi(year)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { EmissionsEntriesApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EmissionsEntriesApiRequest;

  try {
    const data = await api.emissionsEntriesApi(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;EmissionEntry&gt;**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Emission entries for year |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## emissionsExportApi

> EmissionsExportResponse emissionsExportApi(year)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { EmissionsExportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EmissionsExportApiRequest;

  try {
    const data = await api.emissionsExportApi(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**EmissionsExportResponse**](EmissionsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Emissions CSV export |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## emissionsFactorsApi

> Array&lt;EmissionFactorResponse&gt; emissionsFactorsApi()



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { EmissionsFactorsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  try {
    const data = await api.emissionsFactorsApi();
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

[**Array&lt;EmissionFactorResponse&gt;**](EmissionFactorResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Builtin emission factors |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## emissionsReportApi

> EmissionsReport emissionsReportApi(year)



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { EmissionsReportApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  const body = {
    // number
    year: 56,
  } satisfies EmissionsReportApiRequest;

  try {
    const data = await api.emissionsReportApi(body);
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
| **year** | `number` |  | [Defaults to `undefined`] |

### Return type

[**EmissionsReport**](EmissionsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Emissions report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## emissionsTargetsApi

> Array&lt;EmissionTarget&gt; emissionsTargetsApi()



### Example

```ts
import {
  Configuration,
  EmissionsApi,
} from '@simplebilly/api';
import type { EmissionsTargetsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmissionsApi(config);

  try {
    const data = await api.emissionsTargetsApi();
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

[**Array&lt;EmissionTarget&gt;**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Emission reduction targets (ESRS E1-4) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

