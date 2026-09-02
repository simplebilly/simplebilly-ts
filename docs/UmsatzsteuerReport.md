
# UmsatzsteuerReport


## Properties

Name | Type
------------ | -------------
`generatedAt` | string
`inputTax` | [Array&lt;VatDetail&gt;](VatDetail.md)
`outputTax` | [Array&lt;VatDetail&gt;](VatDetail.md)
`period` | string
`totalInputTax` | string
`totalOutputTax` | string
`vatPayable` | string
`vatRefund` | string

## Example

```typescript
import type { UmsatzsteuerReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "generatedAt": null,
  "inputTax": null,
  "outputTax": null,
  "period": null,
  "totalInputTax": null,
  "totalOutputTax": null,
  "vatPayable": null,
  "vatRefund": null,
} satisfies UmsatzsteuerReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UmsatzsteuerReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


