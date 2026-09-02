# GezApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**gezApi**](GezApi.md#gezapi) | **GET** /api/v1/bookkeeping/gez |  |



## gezApi

> GezReport gezApi(jahr, betriebsstaetten, kfz, hotelzimmer, beschaefigte)



### Example

```ts
import {
  Configuration,
  GezApi,
} from '@simplebilly/api';
import type { GezApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new GezApi(config);

  const body = {
    // number (optional)
    jahr: 56,
    // string | Liste der Betriebsstätten als JSON, z.B. `[{\"name\":\"Filiale 1\",\"beschaefigte\":12}]`. (optional)
    betriebsstaetten: betriebsstaetten_example,
    // number | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). (optional)
    kfz: 789,
    // number | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. (optional)
    hotelzimmer: 789,
    // number | Gesamtzahl der Beschäftigten (verwendet nur, wenn `betriebsstaetten` fehlt; dann wird eine einzelne Betriebsstätte angenommen). (optional)
    beschaefigte: 789,
  } satisfies GezApiRequest;

  try {
    const data = await api.gezApi(body);
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
| **jahr** | `number` |  | [Optional] [Defaults to `undefined`] |
| **betriebsstaetten** | `string` | Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [Optional] [Defaults to `undefined`] |
| **kfz** | `number` | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [Optional] [Defaults to `undefined`] |
| **hotelzimmer** | `number` | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [Optional] [Defaults to `undefined`] |
| **beschaefigte** | `number` | Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [Optional] [Defaults to `undefined`] |

### Return type

[**GezReport**](GezReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Rundfunkbeitrag (GEZ) Berechnung nach § 5 RBStV |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

