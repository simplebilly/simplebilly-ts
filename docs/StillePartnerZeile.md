
# StillePartnerZeile


## Properties

Name | Type
------------ | -------------
`auseinandersetzungsguthaben` | string
`gewinnanteil` | string
`gewinnvortrag` | string
`hinweis` | string
`instrumentType` | string
`kest` | string
`name` | string
`verlustVerrechnungskonto` | string
`verlustanteil` | string

## Example

```typescript
import type { StillePartnerZeile } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "auseinandersetzungsguthaben": null,
  "gewinnanteil": null,
  "gewinnvortrag": null,
  "hinweis": null,
  "instrumentType": null,
  "kest": null,
  "name": null,
  "verlustVerrechnungskonto": null,
  "verlustanteil": null,
} satisfies StillePartnerZeile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StillePartnerZeile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


