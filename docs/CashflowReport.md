
# CashflowReport


## Properties

Name | Type
------------ | -------------
`closingBalance` | number
`financingCashflow` | number
`investingCashflow` | number
`netCashflow` | number
`openingBalance` | number
`operatingCashflow` | number
`period` | string

## Example

```typescript
import type { CashflowReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "closingBalance": null,
  "financingCashflow": null,
  "investingCashflow": null,
  "netCashflow": null,
  "openingBalance": null,
  "operatingCashflow": null,
  "period": null,
} satisfies CashflowReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CashflowReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


