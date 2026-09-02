
# GroupFigureUpdate


## Properties

Name | Type
------------ | -------------
`bilanzsumme` | string
`exemptionClaimed` | boolean
`mitarbeiter` | number
`nettoUmsatz` | string
`parentName` | string
`parentSitus` | string

## Example

```typescript
import type { GroupFigureUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bilanzsumme": null,
  "exemptionClaimed": null,
  "mitarbeiter": null,
  "nettoUmsatz": null,
  "parentName": null,
  "parentSitus": null,
} satisfies GroupFigureUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GroupFigureUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


