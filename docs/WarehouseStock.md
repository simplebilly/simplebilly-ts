
# WarehouseStock


## Properties

Name | Type
------------ | -------------
`batchNumber` | string
`binLocation` | string
`expiryDate` | Date
`productId` | string
`quantity` | number
`serialNumbers` | any
`warehouseId` | string

## Example

```typescript
import type { WarehouseStock } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "batchNumber": null,
  "binLocation": null,
  "expiryDate": null,
  "productId": null,
  "quantity": null,
  "serialNumbers": null,
  "warehouseId": null,
} satisfies WarehouseStock

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WarehouseStock
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


