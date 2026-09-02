
# EBilanzReport


## Properties

Name | Type
------------ | -------------
`accountOverview` | [Array&lt;AccountOverview&gt;](AccountOverview.md)
`balanceSheet` | [BalanceSheet](BalanceSheet.md)
`generatedAt` | string
`incomeStatement` | [IncomeStatement](IncomeStatement.md)
`period` | string
`vatSummary` | [VatSummary](VatSummary.md)

## Example

```typescript
import type { EBilanzReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountOverview": null,
  "balanceSheet": null,
  "generatedAt": null,
  "incomeStatement": null,
  "period": null,
  "vatSummary": null,
} satisfies EBilanzReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EBilanzReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


