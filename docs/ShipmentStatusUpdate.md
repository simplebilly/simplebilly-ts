
# ShipmentStatusUpdate


## Properties

Name | Type
------------ | -------------
`deliveredAt` | string
`signedBy` | string
`status` | string
`trackingNumber` | string

## Example

```typescript
import type { ShipmentStatusUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "deliveredAt": null,
  "signedBy": null,
  "status": null,
  "trackingNumber": null,
} satisfies ShipmentStatusUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShipmentStatusUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


