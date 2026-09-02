
# AllocatePaymentRequest


## Properties

Name | Type
------------ | -------------
`amount` | number
`invoiceId` | string
`paymentId` | string

## Example

```typescript
import type { AllocatePaymentRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amount": null,
  "invoiceId": null,
  "paymentId": null,
} satisfies AllocatePaymentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AllocatePaymentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


