# TrainingsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMyTrainings**](TrainingsApi.md#getmytrainings) | **GET** /api/v1/trainings/me |  |
| [**getTrainingContent**](TrainingsApi.md#gettrainingcontent) | **GET** /api/v1/trainings/content/{code} |  |
| [**getTrainingOverview**](TrainingsApi.md#gettrainingoverview) | **GET** /api/v1/trainings/overview |  |
| [**submitTrainingResult**](TrainingsApi.md#submittrainingresult) | **POST** /api/v1/trainings/submit-result |  |



## getMyTrainings

> Array&lt;MyTrainingItem&gt; getMyTrainings()



### Example

```ts
import {
  Configuration,
  TrainingsApi,
} from '@simplebilly/api';
import type { GetMyTrainingsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingsApi(config);

  try {
    const data = await api.getMyTrainings();
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

[**Array&lt;MyTrainingItem&gt;**](MyTrainingItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Required trainings for the current employee |  -  |
| **404** | No employee linked to user |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTrainingContent

> TrainingContent getTrainingContent(code)



### Example

```ts
import {
  Configuration,
  TrainingsApi,
} from '@simplebilly/api';
import type { GetTrainingContentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingsApi(config);

  const body = {
    // string | Training code, e.g. data_privacy
    code: code_example,
  } satisfies GetTrainingContentRequest;

  try {
    const data = await api.getTrainingContent(body);
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
| **code** | `string` | Training code, e.g. data_privacy | [Defaults to `undefined`] |

### Return type

[**TrainingContent**](TrainingContent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Interactive training content for the frontend player |  -  |
| **404** | Unknown training code |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTrainingOverview

> Array&lt;HrTrainingOverview&gt; getTrainingOverview()



### Example

```ts
import {
  Configuration,
  TrainingsApi,
} from '@simplebilly/api';
import type { GetTrainingOverviewRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingsApi(config);

  try {
    const data = await api.getTrainingOverview();
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

[**Array&lt;HrTrainingOverview&gt;**](HrTrainingOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | HR overview of assigned trainings |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## submitTrainingResult

> SubmitResultResponse submitTrainingResult(submitResultDto)



### Example

```ts
import {
  Configuration,
  TrainingsApi,
} from '@simplebilly/api';
import type { SubmitTrainingResultRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingsApi(config);

  const body = {
    // SubmitResultDto
    submitResultDto: ...,
  } satisfies SubmitTrainingResultRequest;

  try {
    const data = await api.submitTrainingResult(body);
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
| **submitResultDto** | [SubmitResultDto](SubmitResultDto.md) |  | |

### Return type

[**SubmitResultResponse**](SubmitResultResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Result recorded |  -  |
| **400** | Invalid score or training |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

