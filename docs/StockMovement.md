
# StockMovement


## Properties

Name | Type
------------ | -------------
`delta` | number
`movementType` | [MovementType](MovementType.md)
`productId` | string
`quantity` | number
`reason` | string
`referenceId` | string
`referenceType` | [ReferenceType](ReferenceType.md)
`warehouseId` | string

## Example

```typescript
import type { StockMovement } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "delta": null,
  "movementType": null,
  "productId": null,
  "quantity": null,
  "reason": null,
  "referenceId": null,
  "referenceType": null,
  "warehouseId": null,
} satisfies StockMovement

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StockMovement
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


