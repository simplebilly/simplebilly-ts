# SupportChannelApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createChannelApi**](SupportChannelApi.md#createchannelapi) | **POST** /api/v1/support/channels |  |
| [**deleteChannelApi**](SupportChannelApi.md#deletechannelapi) | **DELETE** /api/v1/support/channels/{channel_id} |  |
| [**listChannelsApi**](SupportChannelApi.md#listchannelsapi) | **GET** /api/v1/support/channels |  |
| [**updateChannelApi**](SupportChannelApi.md#updatechannelapi) | **PUT** /api/v1/support/channels/{channel_id} |  |



## createChannelApi

> SupportChannel createChannelApi(createChannelDto)



### Example

```ts
import {
  Configuration,
  SupportChannelApi,
} from '@simplebilly/api';
import type { CreateChannelApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportChannelApi(config);

  const body = {
    // CreateChannelDto
    createChannelDto: ...,
  } satisfies CreateChannelApiRequest;

  try {
    const data = await api.createChannelApi(body);
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
| **createChannelDto** | [CreateChannelDto](CreateChannelDto.md) |  | |

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Channel created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteChannelApi

> deleteChannelApi(channelId)



### Example

```ts
import {
  Configuration,
  SupportChannelApi,
} from '@simplebilly/api';
import type { DeleteChannelApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportChannelApi(config);

  const body = {
    // string
    channelId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteChannelApiRequest;

  try {
    const data = await api.deleteChannelApi(body);
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
| **channelId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Channel deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listChannelsApi

> Array&lt;SupportChannel&gt; listChannelsApi()



### Example

```ts
import {
  Configuration,
  SupportChannelApi,
} from '@simplebilly/api';
import type { ListChannelsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportChannelApi(config);

  try {
    const data = await api.listChannelsApi();
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

[**Array&lt;SupportChannel&gt;**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of channels |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateChannelApi

> SupportChannel updateChannelApi(channelId, updateChannelDto)



### Example

```ts
import {
  Configuration,
  SupportChannelApi,
} from '@simplebilly/api';
import type { UpdateChannelApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SupportChannelApi(config);

  const body = {
    // string
    channelId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // UpdateChannelDto
    updateChannelDto: ...,
  } satisfies UpdateChannelApiRequest;

  try {
    const data = await api.updateChannelApi(body);
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
| **channelId** | `string` |  | [Defaults to `undefined`] |
| **updateChannelDto** | [UpdateChannelDto](UpdateChannelDto.md) |  | |

### Return type

[**SupportChannel**](SupportChannel.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Channel updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

