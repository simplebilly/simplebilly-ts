
# KstErgebnis


## Properties

Name | Type
------------ | -------------
`gesamt` | string
`gesamtbelastung` | string
`gewerbesteuer` | string
`gewinn` | string
`istKapitalgesellschaft` | boolean
`jahr` | number
`koerperschaftsteuer` | string
`solidaritaetszuschlag` | string

## Example

```typescript
import type { KstErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "gesamt": null,
  "gesamtbelastung": null,
  "gewerbesteuer": null,
  "gewinn": null,
  "istKapitalgesellschaft": null,
  "jahr": null,
  "koerperschaftsteuer": null,
  "solidaritaetszuschlag": null,
} satisfies KstErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KstErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


