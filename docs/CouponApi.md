# CouponApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**couponRestore**](CouponApi.md#couponrestore) | **POST** /api/v1/coupons/{coupon_id}/restore |  |
| [**createCoupon**](CouponApi.md#createcoupon) | **POST** /api/v1/coupons |  |
| [**deleteCoupon**](CouponApi.md#deletecoupon) | **DELETE** /api/v1/coupons/{coupon_id} |  |
| [**getCoupon**](CouponApi.md#getcoupon) | **GET** /api/v1/coupons/{coupon_id} |  |
| [**listCoupons**](CouponApi.md#listcoupons) | **GET** /api/v1/coupons/ |  |
| [**updateCoupon**](CouponApi.md#updatecoupon) | **PUT** /api/v1/coupons/{coupon_id} |  |



## couponRestore

> Coupon couponRestore(couponId)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { CouponRestoreRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // string
    couponId: couponId_example,
  } satisfies CouponRestoreRequest;

  try {
    const data = await api.couponRestore(body);
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
| **couponId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Coupon**](Coupon.md)

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


## createCoupon

> Coupon createCoupon(couponCreate)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { CreateCouponRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // CouponCreate
    couponCreate: ...,
  } satisfies CreateCouponRequest;

  try {
    const data = await api.createCoupon(body);
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
| **couponCreate** | [CouponCreate](CouponCreate.md) |  | |

### Return type

[**Coupon**](Coupon.md)

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


## deleteCoupon

> deleteCoupon(couponId)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { DeleteCouponRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // string
    couponId: couponId_example,
  } satisfies DeleteCouponRequest;

  try {
    const data = await api.deleteCoupon(body);
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
| **couponId** | `string` |  | [Defaults to `undefined`] |

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


## getCoupon

> Coupon getCoupon(couponId)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { GetCouponRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // string
    couponId: couponId_example,
  } satisfies GetCouponRequest;

  try {
    const data = await api.getCoupon(body);
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
| **couponId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Coupon**](Coupon.md)

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


## listCoupons

> Array&lt;Coupon&gt; listCoupons(page, pageSize, isActive, code, discountType)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { ListCouponsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
    // boolean (optional)
    isActive: true,
    // string (optional)
    code: code_example,
    // string (optional)
    discountType: discountType_example,
  } satisfies ListCouponsRequest;

  try {
    const data = await api.listCoupons(body);
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
| **isActive** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **code** | `string` |  | [Optional] [Defaults to `undefined`] |
| **discountType** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;Coupon&gt;**](Coupon.md)

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


## updateCoupon

> Coupon updateCoupon(couponId, couponUpdate)



### Example

```ts
import {
  Configuration,
  CouponApi,
} from '@simplebilly/api';
import type { UpdateCouponRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CouponApi(config);

  const body = {
    // string
    couponId: couponId_example,
    // CouponUpdate
    couponUpdate: ...,
  } satisfies UpdateCouponRequest;

  try {
    const data = await api.updateCoupon(body);
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
| **couponId** | `string` |  | [Defaults to `undefined`] |
| **couponUpdate** | [CouponUpdate](CouponUpdate.md) |  | |

### Return type

[**Coupon**](Coupon.md)

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

