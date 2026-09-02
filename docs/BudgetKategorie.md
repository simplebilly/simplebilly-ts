
# BudgetKategorie


## Properties

Name | Type
------------ | -------------
`budget` | string
`differenz` | string
`goal` | string
`ist` | string
`kategorie` | string

## Example

```typescript
import type { BudgetKategorie } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "budget": null,
  "differenz": null,
  "goal": null,
  "ist": null,
  "kategorie": null,
} satisfies BudgetKategorie

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BudgetKategorie
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


