
# EuerZeile


## Properties

Name | Type
------------ | -------------
`abschnitt` | string
`betrag` | string
`bezeichnung` | string
`zeile` | number

## Example

```typescript
import type { EuerZeile } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "abschnitt": null,
  "betrag": null,
  "bezeichnung": null,
  "zeile": null,
} satisfies EuerZeile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EuerZeile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


