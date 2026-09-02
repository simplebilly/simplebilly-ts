
# PayrollSummaryItem


## Properties

Name | Type
------------ | -------------
`employeeCount` | number
`month` | string
`status` | [PayrollRunStatus](PayrollRunStatus.md)
`totalEmployerCost` | string
`totalGross` | string
`totalNet` | string
`year` | number

## Example

```typescript
import type { PayrollSummaryItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "employeeCount": null,
  "month": null,
  "status": null,
  "totalEmployerCost": null,
  "totalGross": null,
  "totalNet": null,
  "year": null,
} satisfies PayrollSummaryItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollSummaryItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


