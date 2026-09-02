
# EksErgebnis


## Properties

Name | Type
------------ | -------------
`gesamtergebnis` | string
`monate` | [Array&lt;EksMonatsWert&gt;](EksMonatsWert.md)
`prognoseNaechste6Monate` | string
`summeAusgaben` | string
`summeEinnahmen` | string
`zeitraumBis` | string
`zeitraumVon` | string

## Example

```typescript
import type { EksErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "gesamtergebnis": null,
  "monate": null,
  "prognoseNaechste6Monate": null,
  "summeAusgaben": null,
  "summeEinnahmen": null,
  "zeitraumBis": null,
  "zeitraumVon": null,
} satisfies EksErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EksErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


