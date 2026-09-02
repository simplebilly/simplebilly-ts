# LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLegalDocuments**](LegalDocumentApi.md#getlegaldocuments) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access. |
| [**resetLegalDocuments**](LegalDocumentApi.md#resetlegaldocuments) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list. |
| [**upsertLegalDocuments**](LegalDocumentApi.md#upsertlegaldocuments) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list. |



## getLegalDocuments

> Array&lt;LegalDocument&gt; getLegalDocuments()

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Example

```ts
import {
  Configuration,
  LegalDocumentApi,
} from '@simplebilly/api';
import type { GetLegalDocumentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LegalDocumentApi(config);

  try {
    const data = await api.getLegalDocuments();
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

[**Array&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | All legal documents of the tenant |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resetLegalDocuments

> Array&lt;LegalDocument&gt; resetLegalDocuments(legalDocumentReset)

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Example

```ts
import {
  Configuration,
  LegalDocumentApi,
} from '@simplebilly/api';
import type { ResetLegalDocumentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LegalDocumentApi(config);

  const body = {
    // LegalDocumentReset
    legalDocumentReset: ...,
  } satisfies ResetLegalDocumentsRequest;

  try {
    const data = await api.resetLegalDocuments(body);
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
| **legalDocumentReset** | [LegalDocumentReset](LegalDocumentReset.md) |  | |

### Return type

[**Array&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reset legal documents |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## upsertLegalDocuments

> Array&lt;LegalDocument&gt; upsertLegalDocuments(legalDocumentUpsert)

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Example

```ts
import {
  Configuration,
  LegalDocumentApi,
} from '@simplebilly/api';
import type { UpsertLegalDocumentsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LegalDocumentApi(config);

  const body = {
    // Array<LegalDocumentUpsert>
    legalDocumentUpsert: ...,
  } satisfies UpsertLegalDocumentsRequest;

  try {
    const data = await api.upsertLegalDocuments(body);
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
| **legalDocumentUpsert** | `Array<LegalDocumentUpsert>` |  | |

### Return type

[**Array&lt;LegalDocument&gt;**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Saved legal documents |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

