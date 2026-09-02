
# PayrollSummary


## Properties

Name | Type
------------ | -------------
`firstName` | string
`hourlyGross` | string
`id` | string
`jobTitle` | string
`lastName` | string
`monthlySalary` | string
`months` | [Array&lt;PayrollMonth&gt;](PayrollMonth.md)
`weeklyHours` | string
`year` | number

## Example

```typescript
import type { PayrollSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "firstName": null,
  "hourlyGross": null,
  "id": null,
  "jobTitle": null,
  "lastName": null,
  "monthlySalary": null,
  "months": null,
  "weeklyHours": null,
  "year": null,
} satisfies PayrollSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


