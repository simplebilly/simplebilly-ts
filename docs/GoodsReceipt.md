
# GoodsReceipt


## Properties

Name | Type
------------ | -------------
`grNumber` | string
`lineItems` | any
`notes` | string
`purchaseOrderId` | string
`receiptDate` | Date
`supplierContactId` | string
`supplierName` | string
`warehouseId` | string

## Example

```typescript
import type { GoodsReceipt } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "grNumber": null,
  "lineItems": null,
  "notes": null,
  "purchaseOrderId": null,
  "receiptDate": null,
  "supplierContactId": null,
  "supplierName": null,
  "warehouseId": null,
} satisfies GoodsReceipt

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GoodsReceipt
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


