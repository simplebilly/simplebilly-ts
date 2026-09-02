
# CustomerInfo

Additional information about the customer placing the shipment.

## Properties

Name | Type
------------ | -------------
`annualVolume` | number
`isRegistered` | boolean

## Example

```typescript
import type { CustomerInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "annualVolume": null,
  "isRegistered": null,
} satisfies CustomerInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


