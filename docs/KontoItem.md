
# KontoItem


## Properties

Name | Type
------------ | -------------
`anfangsbestand` | string
`habenUmsatz` | string
`konto` | string
`name` | string
`saldo` | string
`sollUmsatz` | string

## Example

```typescript
import type { KontoItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "anfangsbestand": null,
  "habenUmsatz": null,
  "konto": null,
  "name": null,
  "saldo": null,
  "sollUmsatz": null,
} satisfies KontoItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KontoItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


