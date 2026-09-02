
# KonzernThresholds


## Properties

Name | Type
------------ | -------------
`bilanzsumme` | string
`mitarbeiter` | number
`nettoUmsatz` | string

## Example

```typescript
import type { KonzernThresholds } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bilanzsumme": null,
  "mitarbeiter": null,
  "nettoUmsatz": null,
} satisfies KonzernThresholds

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KonzernThresholds
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


