
# ShippingThresholdUpdate


## Properties

Name | Type
------------ | -------------
`isActive` | boolean
`maxSellable` | number
`name` | string
`notes` | string
`productId` | string
`reserveStock` | number
`warehouseId` | string

## Example

```typescript
import type { ShippingThresholdUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "isActive": null,
  "maxSellable": null,
  "name": null,
  "notes": null,
  "productId": null,
  "reserveStock": null,
  "warehouseId": null,
} satisfies ShippingThresholdUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShippingThresholdUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


