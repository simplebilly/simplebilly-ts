
# DownPaymentInvoice


## Properties

Name | Type
------------ | -------------
`contactId` | string
`contactName` | string
`createdAt` | string
`currency` | string
`id` | string
`notes` | string
`paidAmount` | string
`totalAmount` | string
`voucherDate` | Date
`voucherNumber` | string
`voucherStatus` | string

## Example

```typescript
import type { DownPaymentInvoice } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "contactId": null,
  "contactName": null,
  "createdAt": null,
  "currency": null,
  "id": null,
  "notes": null,
  "paidAmount": null,
  "totalAmount": null,
  "voucherDate": null,
  "voucherNumber": null,
  "voucherStatus": null,
} satisfies DownPaymentInvoice

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DownPaymentInvoice
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


