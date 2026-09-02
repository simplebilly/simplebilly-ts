
# GewerbesteuerErgebnis


## Properties

Name | Type
------------ | -------------
`freibetrag` | string
`gesamtbelastung` | string
`gewerbeertrag` | string
`hebesatz` | string
`jahr` | number
`koerperschaftsteuer` | string
`land` | string
`messbetrag` | string
`steuer` | string
`steuerArt` | string

## Example

```typescript
import type { GewerbesteuerErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "freibetrag": null,
  "gesamtbelastung": null,
  "gewerbeertrag": null,
  "hebesatz": null,
  "jahr": null,
  "koerperschaftsteuer": null,
  "land": null,
  "messbetrag": null,
  "steuer": null,
  "steuerArt": null,
} satisfies GewerbesteuerErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GewerbesteuerErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


