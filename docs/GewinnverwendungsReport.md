
# GewinnverwendungsReport


## Properties

Name | Type
------------ | -------------
`bilanzgewinn` | string
`gesetzlicheRuecklageBestand` | string
`gesetzlicheRuecklageCap` | string
`gesetzlicheRuecklageNach` | string
`gesetzlicheRuecklageSoll` | string
`gezeichnetesKapital` | string
`jahresueberschuss` | string
`year` | number
`zeilen` | [Array&lt;GewinnverwendungsZeile&gt;](GewinnverwendungsZeile.md)

## Example

```typescript
import type { GewinnverwendungsReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bilanzgewinn": null,
  "gesetzlicheRuecklageBestand": null,
  "gesetzlicheRuecklageCap": null,
  "gesetzlicheRuecklageNach": null,
  "gesetzlicheRuecklageSoll": null,
  "gezeichnetesKapital": null,
  "jahresueberschuss": null,
  "year": null,
  "zeilen": null,
} satisfies GewinnverwendungsReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GewinnverwendungsReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


