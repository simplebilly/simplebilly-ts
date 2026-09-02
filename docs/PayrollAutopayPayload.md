
# PayrollAutopayPayload


## Properties

Name | Type
------------ | -------------
`debtorBic` | string
`debtorIban` | string
`debtorName` | string
`executionDate` | Date

## Example

```typescript
import type { PayrollAutopayPayload } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "debtorBic": null,
  "debtorIban": null,
  "debtorName": null,
  "executionDate": null,
} satisfies PayrollAutopayPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollAutopayPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


