# TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**clockInTimeEntry**](TimeEntriesApi.md#clockintimeentry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile). |
| [**clockOutTimeEntry**](TimeEntriesApi.md#clockouttimeentry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry\&#39;s owner, or anyone with &#x60;time_entries:write&#x60;. |
| [**getLaborCosts**](TimeEntriesApi.md#getlaborcosts) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee\&#39;s hourly cost rate. |
| [**listTimeEntries**](TimeEntriesApi.md#listtimeentries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters. |



## clockInTimeEntry

> TimeEntryDto clockInTimeEntry(timeEntryClockIn)

Clock in for the authenticated user (resolved via their employee profile).

### Example

```ts
import {
  Configuration,
  TimeEntriesApi,
} from '@simplebilly/api';
import type { ClockInTimeEntryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimeEntriesApi(config);

  const body = {
    // TimeEntryClockIn
    timeEntryClockIn: ...,
  } satisfies ClockInTimeEntryRequest;

  try {
    const data = await api.clockInTimeEntry(body);
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
| **timeEntryClockIn** | [TimeEntryClockIn](TimeEntryClockIn.md) |  | |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | No employee profile for this user |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## clockOutTimeEntry

> TimeEntryDto clockOutTimeEntry(id, timeEntryClockOut)

Clock out an entry: the entry\&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.

### Example

```ts
import {
  Configuration,
  TimeEntriesApi,
} from '@simplebilly/api';
import type { ClockOutTimeEntryRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimeEntriesApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // TimeEntryClockOut
    timeEntryClockOut: ...,
  } satisfies ClockOutTimeEntryRequest;

  try {
    const data = await api.clockOutTimeEntry(body);
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
| **timeEntryClockOut** | [TimeEntryClockOut](TimeEntryClockOut.md) |  | |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

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
| **403** | Forbidden |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getLaborCosts

> Array&lt;LaborCostRow&gt; getLaborCosts(from, to, groupBy)

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee\&#39;s hourly cost rate.

### Example

```ts
import {
  Configuration,
  TimeEntriesApi,
} from '@simplebilly/api';
import type { GetLaborCostsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimeEntriesApi(config);

  const body = {
    // Date
    from: 2013-10-20,
    // Date
    to: 2013-10-20,
    // string | One of \"employee\", \"order\" or \"day\".
    groupBy: groupBy_example,
  } satisfies GetLaborCostsRequest;

  try {
    const data = await api.getLaborCosts(body);
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
| **from** | `Date` |  | [Defaults to `undefined`] |
| **to** | `Date` |  | [Defaults to `undefined`] |
| **groupBy** | `string` | One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. | [Defaults to `undefined`] |

### Return type

[**Array&lt;LaborCostRow&gt;**](LaborCostRow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTimeEntries

> Array&lt;TimeEntryDto&gt; listTimeEntries(from, to, active, employeeId)

List time entries with optional date-range / active / employee filters.

### Example

```ts
import {
  Configuration,
  TimeEntriesApi,
} from '@simplebilly/api';
import type { ListTimeEntriesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimeEntriesApi(config);

  const body = {
    // Date (optional)
    from: 2013-10-20,
    // Date (optional)
    to: 2013-10-20,
    // boolean | Only currently running shifts (clock_in set, clock_out null). (optional)
    active: true,
    // string (optional)
    employeeId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListTimeEntriesRequest;

  try {
    const data = await api.listTimeEntries(body);
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
| **from** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **to** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **active** | `boolean` | Only currently running shifts (clock_in set, clock_out null). | [Optional] [Defaults to `undefined`] |
| **employeeId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;TimeEntryDto&gt;**](TimeEntryDto.md)

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

