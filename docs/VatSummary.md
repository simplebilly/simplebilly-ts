
# VatSummary


## Properties

Name | Type
------------ | -------------
`inputTaxItems` | [Array&lt;VatItem&gt;](VatItem.md)
`outputTaxItems` | [Array&lt;VatItem&gt;](VatItem.md)
`totalInputTax` | string
`totalOutputTax` | string
`vatDue` | string

## Example

```typescript
import type { VatSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "inputTaxItems": null,
  "outputTaxItems": null,
  "totalInputTax": null,
  "totalOutputTax": null,
  "vatDue": null,
} satisfies VatSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VatSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


