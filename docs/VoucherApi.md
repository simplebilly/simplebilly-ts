# VoucherApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createVoucher**](VoucherApi.md#createvoucher) | **POST** /api/v1/vouchers |  |
| [**deleteVoucher**](VoucherApi.md#deletevoucher) | **DELETE** /api/v1/vouchers/{voucher_id} |  |
| [**getVoucher**](VoucherApi.md#getvoucher) | **GET** /api/v1/vouchers/{voucher_id} |  |
| [**listVouchers**](VoucherApi.md#listvouchers) | **GET** /api/v1/vouchers/ |  |
| [**updateVoucher**](VoucherApi.md#updatevoucher) | **PUT** /api/v1/vouchers/{voucher_id} |  |
| [**voucherRestore**](VoucherApi.md#voucherrestore) | **POST** /api/v1/vouchers/{voucher_id}/restore |  |



## createVoucher

> Voucher createVoucher(voucherCreate)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { CreateVoucherRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // VoucherCreate
    voucherCreate: ...,
  } satisfies CreateVoucherRequest;

  try {
    const data = await api.createVoucher(body);
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
| **voucherCreate** | [VoucherCreate](VoucherCreate.md) |  | |

### Return type

[**Voucher**](Voucher.md)

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


## deleteVoucher

> deleteVoucher(voucherId)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { DeleteVoucherRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // string
    voucherId: voucherId_example,
  } satisfies DeleteVoucherRequest;

  try {
    const data = await api.deleteVoucher(body);
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
| **voucherId** | `string` |  | [Defaults to `undefined`] |

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


## getVoucher

> Voucher getVoucher(voucherId)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { GetVoucherRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // string
    voucherId: voucherId_example,
  } satisfies GetVoucherRequest;

  try {
    const data = await api.getVoucher(body);
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
| **voucherId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Voucher**](Voucher.md)

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


## listVouchers

> Array&lt;Voucher&gt; listVouchers(page, pageSize, voucherType, voucherStatus, contactName, dateFrom, dateTo)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { ListVouchersRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // string (optional)
    voucherType: voucherType_example,
    // string (optional)
    voucherStatus: voucherStatus_example,
    // string (optional)
    contactName: contactName_example,
    // Date (optional)
    dateFrom: 2013-10-20,
    // Date (optional)
    dateTo: 2013-10-20,
  } satisfies ListVouchersRequest;

  try {
    const data = await api.listVouchers(body);
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
| **voucherType** | `string` |  | [Optional] [Defaults to `undefined`] |
| **voucherStatus** | `string` |  | [Optional] [Defaults to `undefined`] |
| **contactName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **dateFrom** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **dateTo** | `Date` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Voucher&gt;**](Voucher.md)

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


## updateVoucher

> Voucher updateVoucher(voucherId, body)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { UpdateVoucherRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // string
    voucherId: voucherId_example,
    // any
    body: ...,
  } satisfies UpdateVoucherRequest;

  try {
    const data = await api.updateVoucher(body);
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
| **voucherId** | `string` |  | [Defaults to `undefined`] |
| **body** | `any` |  | |

### Return type

[**Voucher**](Voucher.md)

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
| **404** | Voucher not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## voucherRestore

> Voucher voucherRestore(voucherId)



### Example

```ts
import {
  Configuration,
  VoucherApi,
} from '@simplebilly/api';
import type { VoucherRestoreRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VoucherApi(config);

  const body = {
    // string
    voucherId: voucherId_example,
  } satisfies VoucherRestoreRequest;

  try {
    const data = await api.voucherRestore(body);
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
| **voucherId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Restored |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

