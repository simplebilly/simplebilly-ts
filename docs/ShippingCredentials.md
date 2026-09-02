
# ShippingCredentials

Per-tenant credentials for real shipping provider APIs (stored in the `shipping` key of the settings JSON blob). Auth is either OAuth client credentials (UPS) or a user-supplied API key (DHL).

## Properties

Name | Type
------------ | -------------
`dhl` | [DhlCredentials](DhlCredentials.md)
`ups` | [UpsCredentials](UpsCredentials.md)

## Example

```typescript
import type { ShippingCredentials } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "dhl": null,
  "ups": null,
} satisfies ShippingCredentials

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShippingCredentials
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


