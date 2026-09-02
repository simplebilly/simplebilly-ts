# PosApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**posBilling**](PosApi.md#posbilling) | **GET** /api/pos/billing |  |
| [**posCreateOrder**](PosApi.md#poscreateorder) | **POST** /api/pos/orders |  |
| [**posCreateRegister**](PosApi.md#poscreateregister) | **POST** /api/pos/registers |  |
| [**posCreateTable**](PosApi.md#poscreatetable) | **POST** /api/pos/tables |  |
| [**posDisableRegister**](PosApi.md#posdisableregister) | **POST** /api/pos/registers/{id}/disable |  |
| [**posFreeTable**](PosApi.md#posfreetable) | **POST** /api/pos/tables/{id}/free |  |
| [**posKasseClosing**](PosApi.md#poskasseclosing) | **POST** /api/pos/kasse/closing |  |
| [**posKasseEntries**](PosApi.md#poskasseentries) | **GET** /api/pos/kasse/entries |  |
| [**posKasseExport**](PosApi.md#poskasseexport) | **GET** /api/pos/kasse/export |  |
| [**posKassePayInOut**](PosApi.md#poskassepayinout) | **POST** /api/pos/kasse/pay-in-out |  |
| [**posListOrders**](PosApi.md#poslistorders) | **GET** /api/pos/orders |  |
| [**posListProducts**](PosApi.md#poslistproducts) | **GET** /api/pos/products |  |
| [**posListRegisters**](PosApi.md#poslistregisters) | **GET** /api/pos/registers |  |
| [**posListTables**](PosApi.md#poslisttables) | **GET** /api/pos/tables |  |
| [**posOrderPrint**](PosApi.md#posorderprint) | **GET** /api/pos/orders/{order_number}/print |  |
| [**posOrderReceipt**](PosApi.md#posorderreceipt) | **GET** /api/pos/orders/{order_number}/receipt |  |
| [**posPayOrder**](PosApi.md#pospayorder) | **POST** /api/pos/orders/{order_number}/pay |  |
| [**posSumupCheckout**](PosApi.md#possumupcheckout) | **POST** /api/pos/sumup/checkout |  |



## posBilling

> any posBilling()



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosBillingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  try {
    const data = await api.posBilling();
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

**any**

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


## posCreateOrder

> any posCreateOrder(body)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosCreateOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // any
    body: ...,
  } satisfies PosCreateOrderRequest;

  try {
    const data = await api.posCreateOrder(body);
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
| **body** | `any` |  | |

### Return type

**any**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## posCreateRegister

> PosRegister posCreateRegister(posRegisterCreate)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosCreateRegisterRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // PosRegisterCreate
    posRegisterCreate: ...,
  } satisfies PosCreateRegisterRequest;

  try {
    const data = await api.posCreateRegister(body);
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
| **posRegisterCreate** | [PosRegisterCreate](PosRegisterCreate.md) |  | |

### Return type

[**PosRegister**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## posCreateTable

> PosTable posCreateTable(posTableCreate)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosCreateTableRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // PosTableCreate
    posTableCreate: ...,
  } satisfies PosCreateTableRequest;

  try {
    const data = await api.posCreateTable(body);
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
| **posTableCreate** | [PosTableCreate](PosTableCreate.md) |  | |

### Return type

[**PosTable**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## posDisableRegister

> PosRegister posDisableRegister(id)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosDisableRegisterRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies PosDisableRegisterRequest;

  try {
    const data = await api.posDisableRegister(body);
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

[**PosRegister**](PosRegister.md)

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


## posFreeTable

> PosTable posFreeTable(id)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosFreeTableRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies PosFreeTableRequest;

  try {
    const data = await api.posFreeTable(body);
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

[**PosTable**](PosTable.md)

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


## posKasseClosing

> any posKasseClosing(body)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosKasseClosingRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // any
    body: ...,
  } satisfies PosKasseClosingRequest;

  try {
    const data = await api.posKasseClosing(body);
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
| **body** | `any` |  | |

### Return type

**any**

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


## posKasseEntries

> any posKasseEntries()



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosKasseEntriesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  try {
    const data = await api.posKasseEntries();
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

**any**

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


## posKasseExport

> any posKasseExport()



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosKasseExportRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  try {
    const data = await api.posKasseExport();
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

**any**

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


## posKassePayInOut

> any posKassePayInOut(body)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosKassePayInOutRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // any
    body: ...,
  } satisfies PosKassePayInOutRequest;

  try {
    const data = await api.posKassePayInOut(body);
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
| **body** | `any` |  | |

### Return type

**any**

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


## posListOrders

> any posListOrders(status)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosListOrdersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string | Filter by order status (optional)
    status: status_example,
  } satisfies PosListOrdersRequest;

  try {
    const data = await api.posListOrders(body);
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
| **status** | `string` | Filter by order status | [Optional] [Defaults to `undefined`] |

### Return type

**any**

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


## posListProducts

> any posListProducts(q)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosListProductsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string | Product search (optional)
    q: q_example,
  } satisfies PosListProductsRequest;

  try {
    const data = await api.posListProducts(body);
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
| **q** | `string` | Product search | [Optional] [Defaults to `undefined`] |

### Return type

**any**

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


## posListRegisters

> Array&lt;PosRegister&gt; posListRegisters()



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosListRegistersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  try {
    const data = await api.posListRegisters();
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

[**Array&lt;PosRegister&gt;**](PosRegister.md)

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


## posListTables

> Array&lt;PosTable&gt; posListTables()



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosListTablesRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  try {
    const data = await api.posListTables();
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

[**Array&lt;PosTable&gt;**](PosTable.md)

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


## posOrderPrint

> any posOrderPrint(orderNumber)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosOrderPrintRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
  } satisfies PosOrderPrintRequest;

  try {
    const data = await api.posOrderPrint(body);
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

### Return type

**any**

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


## posOrderReceipt

> any posOrderReceipt(orderNumber)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosOrderReceiptRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
  } satisfies PosOrderReceiptRequest;

  try {
    const data = await api.posOrderReceipt(body);
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

### Return type

**any**

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


## posPayOrder

> any posPayOrder(orderNumber, body)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosPayOrderRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // string
    orderNumber: orderNumber_example,
    // any
    body: ...,
  } satisfies PosPayOrderRequest;

  try {
    const data = await api.posPayOrder(body);
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
| **body** | `any` |  | |

### Return type

**any**

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


## posSumupCheckout

> any posSumupCheckout(body)



### Example

```ts
import {
  Configuration,
  PosApi,
} from '@simplebilly/api';
import type { PosSumupCheckoutRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PosApi(config);

  const body = {
    // any
    body: ...,
  } satisfies PosSumupCheckoutRequest;

  try {
    const data = await api.posSumupCheckout(body);
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
| **body** | `any` |  | |

### Return type

**any**

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

