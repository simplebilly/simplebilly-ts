
# Payment


## Properties

Name | Type
------------ | -------------
`amount` | string
`attachment` | any
`currency` | string
`customerId` | string
`description` | string
`metadata` | any
`method` | [PaymentMethod](PaymentMethod.md)
`paymentDate` | Date
`reference` | string

## Example

```typescript
import type { Payment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amount": null,
  "attachment": null,
  "currency": null,
  "customerId": null,
  "description": null,
  "metadata": null,
  "method": null,
  "paymentDate": null,
  "reference": null,
} satisfies Payment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Payment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


