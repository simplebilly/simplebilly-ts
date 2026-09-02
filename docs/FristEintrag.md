
# FristEintrag


## Properties

Name | Type
------------ | -------------
`bezeichnung` | string
`faellig` | string
`faelligOriginal` | string
`hinweis` | string
`typ` | string
`zeitraum` | string

## Example

```typescript
import type { FristEintrag } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bezeichnung": null,
  "faellig": null,
  "faelligOriginal": null,
  "hinweis": null,
  "typ": null,
  "zeitraum": null,
} satisfies FristEintrag

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as FristEintrag
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


