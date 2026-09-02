
# DeliveryNoteCreate


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
`title` | string
`voucherDate` | Date
`voucherStatus` | [VoucherStatus](VoucherStatus.md)

## Example

```typescript
import type { DeliveryNoteCreate } from '@simplebilly/api'

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
  "title": null,
  "voucherDate": null,
  "voucherStatus": null,
} satisfies DeliveryNoteCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeliveryNoteCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


