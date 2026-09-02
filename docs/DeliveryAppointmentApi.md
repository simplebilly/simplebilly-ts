# DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDeliveryAppointment**](DeliveryAppointmentApi.md#createdeliveryappointment) | **POST** /api/v1/delivery-appointments |  |
| [**deleteDeliveryAppointment**](DeliveryAppointmentApi.md#deletedeliveryappointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} |  |
| [**getDeliveryAppointment**](DeliveryAppointmentApi.md#getdeliveryappointment) | **GET** /api/v1/delivery-appointments/{appointment_id} |  |
| [**getPublicDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#getpublicdeliveryappointmentstatus) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match. |
| [**listDeliveryAppointments**](DeliveryAppointmentApi.md#listdeliveryappointments) | **GET** /api/v1/delivery-appointments |  |
| [**requestPublicDeliveryAppointment**](DeliveryAppointmentApi.md#requestpublicdeliveryappointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request. |
| [**updateDeliveryAppointment**](DeliveryAppointmentApi.md#updatedeliveryappointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} |  |
| [**updateDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#updatedeliveryappointmentstatus) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status |  |



## createDeliveryAppointment

> DeliveryAppointment createDeliveryAppointment(deliveryAppointmentCreate)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { CreateDeliveryAppointmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // DeliveryAppointmentCreate
    deliveryAppointmentCreate: ...,
  } satisfies CreateDeliveryAppointmentRequest;

  try {
    const data = await api.createDeliveryAppointment(body);
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
| **deliveryAppointmentCreate** | [DeliveryAppointmentCreate](DeliveryAppointmentCreate.md) |  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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


## deleteDeliveryAppointment

> deleteDeliveryAppointment(appointmentId)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { DeleteDeliveryAppointmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // string
    appointmentId: appointmentId_example,
  } satisfies DeleteDeliveryAppointmentRequest;

  try {
    const data = await api.deleteDeliveryAppointment(body);
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
| **appointmentId** | `string` |  | [Defaults to `undefined`] |

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


## getDeliveryAppointment

> DeliveryAppointment getDeliveryAppointment(appointmentId)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { GetDeliveryAppointmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // string
    appointmentId: appointmentId_example,
  } satisfies GetDeliveryAppointmentRequest;

  try {
    const data = await api.getDeliveryAppointment(body);
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
| **appointmentId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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


## getPublicDeliveryAppointmentStatus

> PublicDeliveryAppointmentStatusResponse getPublicDeliveryAppointmentStatus(appointmentId, email, token)

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { GetPublicDeliveryAppointmentStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // string
    appointmentId: appointmentId_example,
    // string
    email: email_example,
    // string
    token: token_example,
  } satisfies GetPublicDeliveryAppointmentStatusRequest;

  try {
    const data = await api.getPublicDeliveryAppointmentStatus(body);
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
| **appointmentId** | `string` |  | [Defaults to `undefined`] |
| **email** | `string` |  | [Defaults to `undefined`] |
| **token** | `string` |  | [Defaults to `undefined`] |

### Return type

[**PublicDeliveryAppointmentStatusResponse**](PublicDeliveryAppointmentStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Appointment status |  -  |
| **404** | Appointment not found or credentials mismatch |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listDeliveryAppointments

> Array&lt;DeliveryAppointment&gt; listDeliveryAppointments(page, pageSize, status, warehouseId, from, to)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { ListDeliveryAppointmentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    status: status_example,
    // string (optional)
    warehouseId: warehouseId_example,
    // Date (optional)
    from: 2013-10-20,
    // Date (optional)
    to: 2013-10-20,
  } satisfies ListDeliveryAppointmentsRequest;

  try {
    const data = await api.listDeliveryAppointments(body);
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
| **warehouseId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **from** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **to** | `Date` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;DeliveryAppointment&gt;**](DeliveryAppointment.md)

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


## requestPublicDeliveryAppointment

> PublicDeliveryAppointmentResponse requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest)

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.

### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { RequestPublicDeliveryAppointmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // PublicDeliveryAppointmentRequest
    publicDeliveryAppointmentRequest: ...,
  } satisfies RequestPublicDeliveryAppointmentRequest;

  try {
    const data = await api.requestPublicDeliveryAppointment(body);
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
| **publicDeliveryAppointmentRequest** | [PublicDeliveryAppointmentRequest](PublicDeliveryAppointmentRequest.md) |  | |

### Return type

[**PublicDeliveryAppointmentResponse**](PublicDeliveryAppointmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Appointment requested |  -  |
| **404** | Warehouse not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateDeliveryAppointment

> DeliveryAppointment updateDeliveryAppointment(appointmentId, body)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { UpdateDeliveryAppointmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // string
    appointmentId: appointmentId_example,
    // any
    body: ...,
  } satisfies UpdateDeliveryAppointmentRequest;

  try {
    const data = await api.updateDeliveryAppointment(body);
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
| **appointmentId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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


## updateDeliveryAppointmentStatus

> DeliveryAppointment updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate)



### Example

```ts
import {
  Configuration,
  DeliveryAppointmentApi,
} from '@simplebilly/api';
import type { UpdateDeliveryAppointmentStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DeliveryAppointmentApi(config);

  const body = {
    // string
    appointmentId: appointmentId_example,
    // AppointmentStatusUpdate
    appointmentStatusUpdate: ...,
  } satisfies UpdateDeliveryAppointmentStatusRequest;

  try {
    const data = await api.updateDeliveryAppointmentStatus(body);
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
| **appointmentId** | `string` |  | [Defaults to `undefined`] |
| **appointmentStatusUpdate** | [AppointmentStatusUpdate](AppointmentStatusUpdate.md) |  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad request / invalid transition |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

