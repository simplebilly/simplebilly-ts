
# OrderConfirmationCreate


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
`taxCondition` | string
`title` | string
`voucherDate` | Date
`voucherStatus` | [VoucherStatus](VoucherStatus.md)

## Example

```typescript
import type { OrderConfirmationCreate } from '@simplebilly/api'

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
  "taxCondition": null,
  "title": null,
  "voucherDate": null,
  "voucherStatus": null,
} satisfies OrderConfirmationCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrderConfirmationCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


