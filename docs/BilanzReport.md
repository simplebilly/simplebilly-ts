
# BilanzReport


## Properties

Name | Type
------------ | -------------
`aktiva` | [Array&lt;BilanzItem&gt;](BilanzItem.md)
`balanced` | boolean
`generatedAt` | string
`passiva` | [Array&lt;BilanzItem&gt;](BilanzItem.md)
`period` | string
`totalAktiva` | string
`totalPassiva` | string

## Example

```typescript
import type { BilanzReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "aktiva": null,
  "balanced": null,
  "generatedAt": null,
  "passiva": null,
  "period": null,
  "totalAktiva": null,
  "totalPassiva": null,
} satisfies BilanzReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BilanzReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


