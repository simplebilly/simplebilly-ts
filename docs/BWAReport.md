
# BWAReport


## Properties

Name | Type
------------ | -------------
`expenses` | [BWAExpenses](BWAExpenses.md)
`generatedAt` | string
`period` | string
`revenue` | [BWARevenue](BWARevenue.md)
`summary` | [BWASummary](BWASummary.md)

## Example

```typescript
import type { BWAReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "expenses": null,
  "generatedAt": null,
  "period": null,
  "revenue": null,
  "summary": null,
} satisfies BWAReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BWAReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


