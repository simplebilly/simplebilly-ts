
# AnlageSKfzHinweis


## Properties

Name | Type
------------ | -------------
`bezeichnung` | string
`kennzeichen` | string
`privatAnteilProzent` | string

## Example

```typescript
import type { AnlageSKfzHinweis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bezeichnung": null,
  "kennzeichen": null,
  "privatAnteilProzent": null,
} satisfies AnlageSKfzHinweis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AnlageSKfzHinweis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


