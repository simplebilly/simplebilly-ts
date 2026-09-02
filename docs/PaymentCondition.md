
# PaymentCondition


## Properties

Name | Type
------------ | -------------
`discountDays` | number
`discountPercentage` | number
`id` | string
`name` | string
`paymentTermDays` | number

## Example

```typescript
import type { PaymentCondition } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "discountDays": null,
  "discountPercentage": null,
  "id": null,
  "name": null,
  "paymentTermDays": null,
} satisfies PaymentCondition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentCondition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


