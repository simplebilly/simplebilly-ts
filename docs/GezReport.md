
# GezReport

Berechnungsergebnis des Rundfunkbeitrags für ein Unternehmen.

## Properties

Name | Type
------------ | -------------
`beitragsfreieKfz` | number
`beitragspflichtigeKfz` | number
`betriebsstaetten` | [Array&lt;BetriebsstaettenDetail&gt;](BetriebsstaettenDetail.md)
`hinweis` | string
`hotelzimmerBeitrag` | string
`jaehrlicherBeitrag` | string
`jahr` | number
`kfzBeitrag` | string
`monatlicherBeitrag` | string
`vierteljaehrlicherBeitrag` | string

## Example

```typescript
import type { GezReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "beitragsfreieKfz": null,
  "beitragspflichtigeKfz": null,
  "betriebsstaetten": null,
  "hinweis": null,
  "hotelzimmerBeitrag": null,
  "jaehrlicherBeitrag": null,
  "jahr": null,
  "kfzBeitrag": null,
  "monatlicherBeitrag": null,
  "vierteljaehrlicherBeitrag": null,
} satisfies GezReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GezReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


