
# BalanceSheet


## Properties

Name | Type
------------ | -------------
`assets` | [Array&lt;BalanceItem&gt;](BalanceItem.md)
`balanced` | boolean
`equityLiabilities` | [Array&lt;BalanceItem&gt;](BalanceItem.md)
`totalAssets` | string
`totalEquityLiabilities` | string

## Example

```typescript
import type { BalanceSheet } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assets": null,
  "balanced": null,
  "equityLiabilities": null,
  "totalAssets": null,
  "totalEquityLiabilities": null,
} satisfies BalanceSheet

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BalanceSheet
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


