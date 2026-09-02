# AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createAttachmentVersion**](AttachmentVersionApi.md#createattachmentversion) | **POST** /api/v1/attachments/{attachment_id}/versions |  |
| [**listAttachmentVersions**](AttachmentVersionApi.md#listattachmentversions) | **GET** /api/v1/attachments/{attachment_id}/versions |  |
| [**restoreAttachmentVersion**](AttachmentVersionApi.md#restoreattachmentversion) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore |  |



## createAttachmentVersion

> AttachmentVersion createAttachmentVersion(attachmentId, newVersionRequest)



### Example

```ts
import {
  Configuration,
  AttachmentVersionApi,
} from '@simplebilly/api';
import type { CreateAttachmentVersionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AttachmentVersionApi(config);

  const body = {
    // string
    attachmentId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // NewVersionRequest
    newVersionRequest: ...,
  } satisfies CreateAttachmentVersionRequest;

  try {
    const data = await api.createAttachmentVersion(body);
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
| **attachmentId** | `string` |  | [Defaults to `undefined`] |
| **newVersionRequest** | [NewVersionRequest](NewVersionRequest.md) |  | |

### Return type

[**AttachmentVersion**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | New current version recorded |  -  |
| **400** | Bad request |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listAttachmentVersions

> Array&lt;AttachmentVersion&gt; listAttachmentVersions(attachmentId)



### Example

```ts
import {
  Configuration,
  AttachmentVersionApi,
} from '@simplebilly/api';
import type { ListAttachmentVersionsRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AttachmentVersionApi(config);

  const body = {
    // string
    attachmentId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListAttachmentVersionsRequest;

  try {
    const data = await api.listAttachmentVersions(body);
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
| **attachmentId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;AttachmentVersion&gt;**](AttachmentVersion.md)

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


## restoreAttachmentVersion

> Attachment restoreAttachmentVersion(attachmentId, versionId)



### Example

```ts
import {
  Configuration,
  AttachmentVersionApi,
} from '@simplebilly/api';
import type { RestoreAttachmentVersionRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AttachmentVersionApi(config);

  const body = {
    // string
    attachmentId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    versionId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies RestoreAttachmentVersionRequest;

  try {
    const data = await api.restoreAttachmentVersion(body);
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
| **attachmentId** | `string` |  | [Defaults to `undefined`] |
| **versionId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attachment restored |  -  |
| **404** | Not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

