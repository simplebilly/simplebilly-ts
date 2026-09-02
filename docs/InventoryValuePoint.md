
# InventoryValuePoint


## Properties

Name | Type
------------ | -------------
`productCount` | number
`recordedAt` | Date
`totalPurchaseValue` | string
`totalSalesValue` | string

## Example

```typescript
import type { InventoryValuePoint } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "productCount": null,
  "recordedAt": null,
  "totalPurchaseValue": null,
  "totalSalesValue": null,
} satisfies InventoryValuePoint

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InventoryValuePoint
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


