
# CostingLine

A single costing line: material cost for one BOM component.

## Properties

Name | Type
------------ | -------------
`lineCost` | string
`name` | string
`productId` | string
`quantityPerUnit` | number
`sku` | string
`totalQuantity` | number
`unitPurchasePrice` | string

## Example

```typescript
import type { CostingLine } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "lineCost": null,
  "name": null,
  "productId": null,
  "quantityPerUnit": null,
  "sku": null,
  "totalQuantity": null,
  "unitPurchasePrice": null,
} satisfies CostingLine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CostingLine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


