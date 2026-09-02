
# EksMonatsWert


## Properties

Name | Type
------------ | -------------
`ausgaben` | string
`einnahmen` | string
`ergebnis` | string
`monat` | string

## Example

```typescript
import type { EksMonatsWert } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "ausgaben": null,
  "einnahmen": null,
  "ergebnis": null,
  "monat": null,
} satisfies EksMonatsWert

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EksMonatsWert
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


