
# KostenEintrag


## Properties

Name | Type
------------ | -------------
`beschreibung` | string
`betrag` | string
`datum` | string
`typ` | string

## Example

```typescript
import type { KostenEintrag } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "beschreibung": null,
  "betrag": null,
  "datum": null,
  "typ": null,
} satisfies KostenEintrag

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KostenEintrag
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


