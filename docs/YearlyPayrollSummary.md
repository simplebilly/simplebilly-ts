
# YearlyPayrollSummary


## Properties

Name | Type
------------ | -------------
`avgEmployeeCount` | number
`months` | [Array&lt;PayrollSummaryItem&gt;](PayrollSummaryItem.md)
`year` | number
`yearlyEmployerCost` | string
`yearlyGross` | string
`yearlyNet` | string

## Example

```typescript
import type { YearlyPayrollSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "avgEmployeeCount": null,
  "months": null,
  "year": null,
  "yearlyEmployerCost": null,
  "yearlyGross": null,
  "yearlyNet": null,
} satisfies YearlyPayrollSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as YearlyPayrollSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


