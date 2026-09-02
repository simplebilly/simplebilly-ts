# CreateSepaDirectDebitApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSepaDirectDebitApi**](CreateSepaDirectDebitApi.md#createsepadirectdebitapi) | **POST** /api/v1/bookkeeping/sepa-direct-debit |  |



## createSepaDirectDebitApi

> SepaDirectDebitResponse createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, creditorBic, debtorBic, description)



### Example

```ts
import {
  Configuration,
  CreateSepaDirectDebitApi,
} from '@simplebilly/api';
import type { CreateSepaDirectDebitApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CreateSepaDirectDebitApi(config);

  const body = {
    // string
    creditorName: creditorName_example,
    // string
    creditorIban: creditorIban_example,
    // string
    creditorId: creditorId_example,
    // string
    mandateId: mandateId_example,
    // string
    mandateDate: mandateDate_example,
    // string
    debtorName: debtorName_example,
    // string
    debtorIban: debtorIban_example,
    // string
    amount: amount_example,
    // string
    collectionDate: collectionDate_example,
    // string (optional)
    creditorBic: creditorBic_example,
    // string (optional)
    debtorBic: debtorBic_example,
    // string (optional)
    description: description_example,
  } satisfies CreateSepaDirectDebitApiRequest;

  try {
    const data = await api.createSepaDirectDebitApi(body);
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
| **creditorName** | `string` |  | [Defaults to `undefined`] |
| **creditorIban** | `string` |  | [Defaults to `undefined`] |
| **creditorId** | `string` |  | [Defaults to `undefined`] |
| **mandateId** | `string` |  | [Defaults to `undefined`] |
| **mandateDate** | `string` |  | [Defaults to `undefined`] |
| **debtorName** | `string` |  | [Defaults to `undefined`] |
| **debtorIban** | `string` |  | [Defaults to `undefined`] |
| **amount** | `string` |  | [Defaults to `undefined`] |
| **collectionDate** | `string` |  | [Defaults to `undefined`] |
| **creditorBic** | `string` |  | [Optional] [Defaults to `undefined`] |
| **debtorBic** | `string` |  | [Optional] [Defaults to `undefined`] |
| **description** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**SepaDirectDebitResponse**](SepaDirectDebitResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SEPA Direct Debit XML |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

