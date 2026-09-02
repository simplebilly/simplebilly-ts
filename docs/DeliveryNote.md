
# DeliveryNote


## Properties

Name | Type
------------ | -------------
`address` | any
`contactId` | string
`contactName` | string
`currency` | string
`deliveryDate` | Date
`deliveryNoteNumber` | string
`files` | any
`introduction` | string
`lineItems` | any
`precedingSalesVoucherId` | string
`precedingSalesVoucherType` | [PrecedingSalesVoucherType](PrecedingSalesVoucherType.md)
`remark` | string
`shippingDate` | Date
`shippingMethod` | string
`subtotal` | string
`title` | string
`totalAmount` | string
`voucherDate` | Date
`voucherStatus` | [VoucherStatus](VoucherStatus.md)

## Example

```typescript
import type { DeliveryNote } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "contactId": null,
  "contactName": null,
  "currency": null,
  "deliveryDate": null,
  "deliveryNoteNumber": null,
  "files": null,
  "introduction": null,
  "lineItems": null,
  "precedingSalesVoucherId": null,
  "precedingSalesVoucherType": null,
  "remark": null,
  "shippingDate": null,
  "shippingMethod": null,
  "subtotal": null,
  "title": null,
  "totalAmount": null,
  "voucherDate": null,
  "voucherStatus": null,
} satisfies DeliveryNote

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeliveryNote
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


