
# EuerZeileDetail


## Properties

Name | Type
------------ | -------------
`abschnitt` | string
`betragGesamt` | string
`bezeichnung` | string
`kategorien` | [Array&lt;EuerKatSumme&gt;](EuerKatSumme.md)
`zeile` | number

## Example

```typescript
import type { EuerZeileDetail } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "abschnitt": null,
  "betragGesamt": null,
  "bezeichnung": null,
  "kategorien": null,
  "zeile": null,
} satisfies EuerZeileDetail

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EuerZeileDetail
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


