
# ReplenishmentSuggestionLine

A single replenishment suggestion.

## Properties

Name | Type
------------ | -------------
`currentStock` | number
`maxStock` | number
`minStock` | number
`productId` | string
`productName` | string
`sku` | string
`sourceAvailable` | number
`sourceWarehouseId` | string
`suggestedQuantity` | number
`targetWarehouseId` | string

## Example

```typescript
import type { ReplenishmentSuggestionLine } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentStock": null,
  "maxStock": null,
  "minStock": null,
  "productId": null,
  "productName": null,
  "sku": null,
  "sourceAvailable": null,
  "sourceWarehouseId": null,
  "suggestedQuantity": null,
  "targetWarehouseId": null,
} satisfies ReplenishmentSuggestionLine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReplenishmentSuggestionLine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


