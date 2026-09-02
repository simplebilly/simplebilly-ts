
# VoucherCreate


## Properties

Name | Type
------------ | -------------
`categoryId` | string
`contactId` | string
`contactName` | string
`currency` | string
`description` | string
`fileAttachments` | any
`lineItems` | any
`metadata` | any
`notes` | string
`openAmount` | string
`paidDate` | Date
`paymentStatus` | [PaymentStatus](PaymentStatus.md)
`taxAmounts` | any
`taxCondition` | string
`totalGrossAmount` | string
`totalNetAmount` | string
`voucherDate` | Date
`voucherNumber` | string
`voucherStatus` | [VoucherStatus](VoucherStatus.md)
`voucherType` | [VoucherType](VoucherType.md)

## Example

```typescript
import type { VoucherCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "categoryId": null,
  "contactId": null,
  "contactName": null,
  "currency": null,
  "description": null,
  "fileAttachments": null,
  "lineItems": null,
  "metadata": null,
  "notes": null,
  "openAmount": null,
  "paidDate": null,
  "paymentStatus": null,
  "taxAmounts": null,
  "taxCondition": null,
  "totalGrossAmount": null,
  "totalNetAmount": null,
  "voucherDate": null,
  "voucherNumber": null,
  "voucherStatus": null,
  "voucherType": null,
} satisfies VoucherCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VoucherCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


