
# CreateShipmentRequest


## Properties

Name | Type
------------ | -------------
`carrier` | string
`service` | string
`weightKg` | number

## Example

```typescript
import type { CreateShipmentRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "carrier": null,
  "service": null,
  "weightKg": null,
} satisfies CreateShipmentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateShipmentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


