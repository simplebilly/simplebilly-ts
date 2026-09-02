
# ProposedAssignment


## Properties

Name | Type
------------ | -------------
`amountPaid` | string
`confidence` | number
`customerId` | string
`invoiceId` | string
`invoiceNumber` | string
`openAmount` | string
`paymentDate` | string
`paymentId` | string
`reason` | string
`reference` | string

## Example

```typescript
import type { ProposedAssignment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amountPaid": null,
  "confidence": null,
  "customerId": null,
  "invoiceId": null,
  "invoiceNumber": null,
  "openAmount": null,
  "paymentDate": null,
  "paymentId": null,
  "reason": null,
  "reference": null,
} satisfies ProposedAssignment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProposedAssignment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


