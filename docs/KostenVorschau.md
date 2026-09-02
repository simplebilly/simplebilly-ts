
# KostenVorschau


## Properties

Name | Type
------------ | -------------
`eintraege` | [Array&lt;KostenEintrag&gt;](KostenEintrag.md)
`gesamt` | string

## Example

```typescript
import type { KostenVorschau } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "eintraege": null,
  "gesamt": null,
} satisfies KostenVorschau

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KostenVorschau
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


