
# EuerErgebnis


## Properties

Name | Type
------------ | -------------
`anlageZugaenge` | string
`gewinnVerlust` | string
`jahr` | number
`summeAusgaben` | string
`summeEinnahmen` | string
`zeilen` | [Array&lt;EuerZeile&gt;](EuerZeile.md)

## Example

```typescript
import type { EuerErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "anlageZugaenge": null,
  "gewinnVerlust": null,
  "jahr": null,
  "summeAusgaben": null,
  "summeEinnahmen": null,
  "zeilen": null,
} satisfies EuerErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EuerErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


