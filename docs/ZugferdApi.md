# ZugferdApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**generateZugferdApi**](ZugferdApi.md#generatezugferdapi) | **GET** /api/v1/invoices/{id}/zugferd |  |



## generateZugferdApi

> generateZugferdApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId)



### Example

```ts
import {
  Configuration,
  ZugferdApi,
} from '@simplebilly/api';
import type { GenerateZugferdApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ZugferdApi(config);

  const body = {
    // string
    id: id_example,
    // string (optional)
    supplierName: supplierName_example,
    // string (optional)
    supplierStreet: supplierStreet_example,
    // string (optional)
    supplierCity: supplierCity_example,
    // string (optional)
    supplierZip: supplierZip_example,
    // string (optional)
    supplierCountry: supplierCountry_example,
    // string (optional)
    supplierVatId: supplierVatId_example,
  } satisfies GenerateZugferdApiRequest;

  try {
    const data = await api.generateZugferdApi(body);
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
| **supplierName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierStreet** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierCity** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierZip** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierCountry** | `string` |  | [Optional] [Defaults to `undefined`] |
| **supplierVatId** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/pdf`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ZUGFeRD/Factur-X hybrid PDF (PDF/A-3 with embedded EN 16931 XML) |  -  |
| **404** | Invoice not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

