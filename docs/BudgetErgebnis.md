
# BudgetErgebnis


## Properties

Name | Type
------------ | -------------
`jahr` | number
`monat` | number
`monatsBudget` | [Array&lt;BudgetKategorie&gt;](BudgetKategorie.md)
`prognoseRestjahr` | [Array&lt;BudgetKategorie&gt;](BudgetKategorie.md)

## Example

```typescript
import type { BudgetErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "jahr": null,
  "monat": null,
  "monatsBudget": null,
  "prognoseRestjahr": null,
} satisfies BudgetErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BudgetErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


