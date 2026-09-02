
# BWASummary


## Properties

Name | Type
------------ | -------------
`grossProfit` | string
`netProfit` | string
`openInvoicesCount` | number
`openInvoicesTotal` | string
`overdueInvoicesCount` | number
`overdueInvoicesTotal` | string
`profitMargin` | number

## Example

```typescript
import type { BWASummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "grossProfit": null,
  "netProfit": null,
  "openInvoicesCount": null,
  "openInvoicesTotal": null,
  "overdueInvoicesCount": null,
  "overdueInvoicesTotal": null,
  "profitMargin": null,
} satisfies BWASummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BWASummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


