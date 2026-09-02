
# PurchaseOrderUpdate


## Properties

Name | Type
------------ | -------------
`currency` | string
`deliveryAddress` | any
`expectedDeliveryDate` | Date
`lineItems` | any
`notes` | string
`orderDate` | Date
`poNumber` | string
`status` | [PurchaseOrderStatus](PurchaseOrderStatus.md)
`supplierContactId` | string
`supplierName` | string
`totalGrossAmount` | string
`totalNetAmount` | string

## Example

```typescript
import type { PurchaseOrderUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "deliveryAddress": null,
  "expectedDeliveryDate": null,
  "lineItems": null,
  "notes": null,
  "orderDate": null,
  "poNumber": null,
  "status": null,
  "supplierContactId": null,
  "supplierName": null,
  "totalGrossAmount": null,
  "totalNetAmount": null,
} satisfies PurchaseOrderUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PurchaseOrderUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


