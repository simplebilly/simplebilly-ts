
# CustomerUpdate


## Properties

Name | Type
------------ | -------------
`address` | any
`contactPerson` | string
`email` | string
`externalOrderNumber` | string
`name` | string
`paymentGracePeriodDays` | number
`phone` | string
`vatId` | string

## Example

```typescript
import type { CustomerUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "contactPerson": null,
  "email": null,
  "externalOrderNumber": null,
  "name": null,
  "paymentGracePeriodDays": null,
  "phone": null,
  "vatId": null,
} satisfies CustomerUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


