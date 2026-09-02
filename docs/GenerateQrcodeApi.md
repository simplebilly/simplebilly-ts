# GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**generateQrcodeApi**](GenerateQrcodeApi.md#generateqrcodeapi) | **GET** /api/v1/invoices/{id}/qrcode |  |



## generateQrcodeApi

> QRCodeResponse generateQrcodeApi(iban, id, holderName, bic, amount, reference, purpose)



### Example

```ts
import {
  Configuration,
  GenerateQrcodeApi,
} from '@simplebilly/api';
import type { GenerateQrcodeApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GenerateQrcodeApi(config);

  const body = {
    // string
    iban: iban_example,
    // string
    id: id_example,
    // string (optional)
    holderName: holderName_example,
    // string (optional)
    bic: bic_example,
    // string (optional)
    amount: amount_example,
    // string (optional)
    reference: reference_example,
    // string (optional)
    purpose: purpose_example,
  } satisfies GenerateQrcodeApiRequest;

  try {
    const data = await api.generateQrcodeApi(body);
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
| **iban** | `string` |  | [Defaults to `undefined`] |
| **id** | `string` |  | [Defaults to `undefined`] |
| **holderName** | `string` |  | [Optional] [Defaults to `undefined`] |
| **bic** | `string` |  | [Optional] [Defaults to `undefined`] |
| **amount** | `string` |  | [Optional] [Defaults to `undefined`] |
| **reference** | `string` |  | [Optional] [Defaults to `undefined`] |
| **purpose** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**QRCodeResponse**](QRCodeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QR Code for invoice payment |  -  |
| **404** | Invoice not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

