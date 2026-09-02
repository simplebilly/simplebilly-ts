
# DeliverableResponse


## Properties

Name | Type
------------ | -------------
`availableStock` | number
`deliverableQuantity` | number
`maxSellable` | number
`productId` | string
`reservedStock` | number
`warehouseId` | string

## Example

```typescript
import type { DeliverableResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "availableStock": null,
  "deliverableQuantity": null,
  "maxSellable": null,
  "productId": null,
  "reservedStock": null,
  "warehouseId": null,
} satisfies DeliverableResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeliverableResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


