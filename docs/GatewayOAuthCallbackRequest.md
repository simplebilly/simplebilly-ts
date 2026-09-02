
# GatewayOAuthCallbackRequest


## Properties

Name | Type
------------ | -------------
`code` | string
`gatewayType` | string
`redirectUri` | string
`state` | string

## Example

```typescript
import type { GatewayOAuthCallbackRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "gatewayType": null,
  "redirectUri": null,
  "state": null,
} satisfies GatewayOAuthCallbackRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GatewayOAuthCallbackRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


