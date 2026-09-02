
# SilentPartner


## Properties

Name | Type
------------ | -------------
`contractDate` | Date
`einlage` | string
`gewinnquotePct` | string
`gewinnvortrag` | string
`instrumentType` | [InstrumentType](InstrumentType.md)
`kestPflichtig` | boolean
`name` | string
`notes` | string
`verlustVerrechnungskonto` | string
`verlustbeteiligung` | boolean

## Example

```typescript
import type { SilentPartner } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "contractDate": null,
  "einlage": null,
  "gewinnquotePct": null,
  "gewinnvortrag": null,
  "instrumentType": null,
  "kestPflichtig": null,
  "name": null,
  "notes": null,
  "verlustVerrechnungskonto": null,
  "verlustbeteiligung": null,
} satisfies SilentPartner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SilentPartner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


