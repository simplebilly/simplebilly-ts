
# GuVReport


## Properties

Name | Type
------------ | -------------
`expenses` | [Array&lt;GuVItem&gt;](GuVItem.md)
`generatedAt` | string
`netIncome` | string
`period` | string
`revenue` | [Array&lt;GuVItem&gt;](GuVItem.md)
`totalExpenses` | string
`totalRevenue` | string

## Example

```typescript
import type { GuVReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "expenses": null,
  "generatedAt": null,
  "netIncome": null,
  "period": null,
  "revenue": null,
  "totalExpenses": null,
  "totalRevenue": null,
} satisfies GuVReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GuVReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


