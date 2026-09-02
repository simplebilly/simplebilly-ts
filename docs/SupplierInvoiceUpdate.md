
# SupplierInvoiceUpdate


## Properties

Name | Type
------------ | -------------
`currency` | string
`goodsReceiptId` | string
`invoiceDate` | Date
`invoiceNumber` | string
`lineItems` | any
`notes` | string
`purchaseOrderId` | string
`status` | [SupplierInvoiceStatus](SupplierInvoiceStatus.md)
`supplierContactId` | string
`supplierName` | string
`totalGrossAmount` | string
`totalNetAmount` | string

## Example

```typescript
import type { SupplierInvoiceUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "goodsReceiptId": null,
  "invoiceDate": null,
  "invoiceNumber": null,
  "lineItems": null,
  "notes": null,
  "purchaseOrderId": null,
  "status": null,
  "supplierContactId": null,
  "supplierName": null,
  "totalGrossAmount": null,
  "totalNetAmount": null,
} satisfies SupplierInvoiceUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SupplierInvoiceUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


