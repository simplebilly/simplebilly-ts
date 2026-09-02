# ShipmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createShipment**](ShipmentApi.md#createshipment) | **POST** /api/v1/shipments |  |
| [**createShipmentFromOrder**](ShipmentApi.md#createshipmentfromorder) | **POST** /api/v1/orders/{order_number}/shipments | Create a real shipment for an order: calls the configured carrier\&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped. |
| [**deleteShipment**](ShipmentApi.md#deleteshipment) | **DELETE** /api/v1/shipments/{shipment_id} |  |
| [**getShipment**](ShipmentApi.md#getshipment) | **GET** /api/v1/shipments/{shipment_id} |  |
| [**listShipments**](ShipmentApi.md#listshipments) | **GET** /api/v1/shipments |  |
| [**trackOrderPublic**](ShipmentApi.md#trackorderpublic) | **POST** /api/v1/public/track | Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API). |
| [**trackShipmentApi**](ShipmentApi.md#trackshipmentapi) | **GET** /api/v1/shipments/{shipment_id}/tracking |  |
| [**updateShipmentStatus**](ShipmentApi.md#updateshipmentstatus) | **PUT** /api/v1/shipments/{shipment_id}/status |  |



## createShipment

> Shipment createShipment(shipment)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { CreateShipmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // Shipment
    shipment: ...,
  } satisfies CreateShipmentRequest;

  try {
    const data = await api.createShipment(body);
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
| **shipment** | [Shipment](Shipment.md) |  | |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Shipment created |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createShipmentFromOrder

> Shipment createShipmentFromOrder(orderNumber, createShipmentRequest)

Create a real shipment for an order: calls the configured carrier\&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.

### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { CreateShipmentFromOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
    // CreateShipmentRequest
    createShipmentRequest: ...,
  } satisfies CreateShipmentFromOrderRequest;

  try {
    const data = await api.createShipmentFromOrder(body);
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
| **orderNumber** | `string` |  | [Defaults to `undefined`] |
| **createShipmentRequest** | [CreateShipmentRequest](CreateShipmentRequest.md) |  | |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Shipment created via carrier API |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteShipment

> deleteShipment(shipmentId)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { DeleteShipmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // string
    shipmentId: shipmentId_example,
  } satisfies DeleteShipmentRequest;

  try {
    const data = await api.deleteShipment(body);
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
| **shipmentId** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Shipment deleted |  -  |
| **404** | Shipment not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getShipment

> Shipment getShipment(shipmentId)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { GetShipmentRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // string
    shipmentId: shipmentId_example,
  } satisfies GetShipmentRequest;

  try {
    const data = await api.getShipment(body);
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
| **shipmentId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Shipment found |  -  |
| **404** | Shipment not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listShipments

> Array&lt;Shipment&gt; listShipments(page, pageSize, search, includeDeleted)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { ListShipmentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // number (optional)
    page: 1,
    // number (optional)
    pageSize: 56,
    // string (optional)
    search: search_example,
    // boolean | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)
    includeDeleted: true,
  } satisfies ListShipmentsRequest;

  try {
    const data = await api.listShipments(body);
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
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **includeDeleted** | `boolean` | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Shipment&gt;**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Shipments found |  -  |
| **400** | Bad request |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## trackOrderPublic

> TrackOrderResponse trackOrderPublic(trackOrderRequest)

Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).

### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { TrackOrderPublicRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // TrackOrderRequest
    trackOrderRequest: ...,
  } satisfies TrackOrderPublicRequest;

  try {
    const data = await api.trackOrderPublic(body);
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
| **trackOrderRequest** | [TrackOrderRequest](TrackOrderRequest.md) |  | |

### Return type

[**TrackOrderResponse**](TrackOrderResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order tracking info |  -  |
| **404** | Order not found or email mismatch |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## trackShipmentApi

> TrackingInfo trackShipmentApi(shipmentId)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { TrackShipmentApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // string
    shipmentId: shipmentId_example,
  } satisfies TrackShipmentApiRequest;

  try {
    const data = await api.trackShipmentApi(body);
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
| **shipmentId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**TrackingInfo**](TrackingInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Live tracking info |  -  |
| **404** | Shipment not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateShipmentStatus

> Shipment updateShipmentStatus(shipmentId, shipmentStatusUpdate)



### Example

```ts
import {
  Configuration,
  ShipmentApi,
} from '@simplebilly/api';
import type { UpdateShipmentStatusRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ShipmentApi(config);

  const body = {
    // string
    shipmentId: shipmentId_example,
    // ShipmentStatusUpdate
    shipmentStatusUpdate: ...,
  } satisfies UpdateShipmentStatusRequest;

  try {
    const data = await api.updateShipmentStatus(body);
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
| **shipmentId** | `string` |  | [Defaults to `undefined`] |
| **shipmentStatusUpdate** | [ShipmentStatusUpdate](ShipmentStatusUpdate.md) |  | |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Status updated |  -  |
| **404** | Shipment not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

