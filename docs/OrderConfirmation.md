
# OrderConfirmation


## Properties

Name | Type
------------ | -------------
`address` | any
`confirmationNumber` | string
`contactId` | string
`contactName` | string
`currency` | string
`files` | any
`introduction` | string
`lineItems` | any
`precedingSalesVoucherId` | string
`precedingSalesVoucherType` | [PrecedingSalesVoucherType](PrecedingSalesVoucherType.md)
`remark` | string
`subtotal` | string
`taxCondition` | string
`title` | string
`totalAmount` | string
`totalTax` | string
`voucherDate` | Date
`voucherStatus` | [VoucherStatus](VoucherStatus.md)

## Example

```typescript
import type { OrderConfirmation } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "confirmationNumber": null,
  "contactId": null,
  "contactName": null,
  "currency": null,
  "files": null,
  "introduction": null,
  "lineItems": null,
  "precedingSalesVoucherId": null,
  "precedingSalesVoucherType": null,
  "remark": null,
  "subtotal": null,
  "taxCondition": null,
  "title": null,
  "totalAmount": null,
  "totalTax": null,
  "voucherDate": null,
  "voucherStatus": null,
} satisfies OrderConfirmation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrderConfirmation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


