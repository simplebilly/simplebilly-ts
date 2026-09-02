# JobApplicationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**applyPublic**](JobApplicationApi.md#applypublic) | **POST** /api/v1/public/jobs/{posting_id}/apply |  |
| [**deleteJobApplication**](JobApplicationApi.md#deletejobapplication) | **DELETE** /api/v1/job-applications/{application_id} |  |
| [**downloadCv**](JobApplicationApi.md#downloadcv) | **GET** /api/v1/job-applications/{application_id}/cv |  |
| [**getJobApplication**](JobApplicationApi.md#getjobapplication) | **GET** /api/v1/job-applications/{application_id} |  |
| [**inboundEmail**](JobApplicationApi.md#inboundemail) | **POST** /api/v1/public/jobs/inbound-email | Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox. |
| [**listJobApplications**](JobApplicationApi.md#listjobapplications) | **GET** /api/v1/job-applications |  |
| [**listPublicPostings**](JobApplicationApi.md#listpublicpostings) | **GET** /api/v1/public/jobs |  |
| [**scoreJobApplication**](JobApplicationApi.md#scorejobapplication) | **POST** /api/v1/job-applications/{application_id}/score |  |
| [**updateJobApplicationStatus**](JobApplicationApi.md#updatejobapplicationstatus) | **PATCH** /api/v1/job-applications/{application_id}/status |  |



## applyPublic

> applyPublic(postingId)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { ApplyPublicRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    postingId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ApplyPublicRequest;

  try {
    const data = await api.applyPublic(body);
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
| **postingId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Application received |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteJobApplication

> JobApplication deleteJobApplication(applicationId)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { DeleteJobApplicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    applicationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteJobApplicationRequest;

  try {
    const data = await api.deleteJobApplication(body);
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
| **applicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Soft-deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## downloadCv

> downloadCv(applicationId)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { DownloadCvRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    applicationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DownloadCvRequest;

  try {
    const data = await api.downloadCv(body);
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
| **applicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CV file |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getJobApplication

> JobApplication getJobApplication(applicationId)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { GetJobApplicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    applicationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetJobApplicationRequest;

  try {
    const data = await api.getJobApplication(body);
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
| **applicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Application |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## inboundEmail

> inboundEmail()

Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox.

### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { InboundEmailRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  try {
    const data = await api.inboundEmail();
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

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Application received |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listJobApplications

> Array&lt;JobApplication&gt; listJobApplications(postingId, status, page, pageSize)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { ListJobApplicationsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string (optional)
    postingId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    status: status_example,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
  } satisfies ListJobApplicationsRequest;

  try {
    const data = await api.listJobApplications(body);
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
| **postingId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;JobApplication&gt;**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Applications list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPublicPostings

> Array&lt;PublicPosting&gt; listPublicPostings()



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { ListPublicPostingsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  try {
    const data = await api.listPublicPostings();
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

[**Array&lt;PublicPosting&gt;**](PublicPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Published postings |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## scoreJobApplication

> JobApplication scoreJobApplication(applicationId)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { ScoreJobApplicationRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    applicationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ScoreJobApplicationRequest;

  try {
    const data = await api.scoreJobApplication(body);
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
| **applicationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Scored |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateJobApplicationStatus

> JobApplication updateJobApplicationStatus(applicationId, applicationStatusDto)



### Example

```ts
import {
  Configuration,
  JobApplicationApi,
} from '@simplebilly/api';
import type { UpdateJobApplicationStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new JobApplicationApi(config);

  const body = {
    // string
    applicationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // ApplicationStatusDto
    applicationStatusDto: ...,
  } satisfies UpdateJobApplicationStatusRequest;

  try {
    const data = await api.updateJobApplicationStatus(body);
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
| **applicationId** | `string` |  | [Defaults to `undefined`] |
| **applicationStatusDto** | [ApplicationStatusDto](ApplicationStatusDto.md) |  | |

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

