
# PayrollCreatePayload


## Properties

Name | Type
------------ | -------------
`employeeIds` | Array&lt;string&gt;
`extraPayments` | [Array&lt;ExtraPayment&gt;](ExtraPayment.md)
`month` | number
`year` | number

## Example

```typescript
import type { PayrollCreatePayload } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "employeeIds": null,
  "extraPayments": null,
  "month": null,
  "year": null,
} satisfies PayrollCreatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollCreatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


