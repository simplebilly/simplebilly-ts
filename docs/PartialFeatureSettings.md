
# PartialFeatureSettings

Partial feature toggles: `None` keeps the company-type default, `Some` overrides it.

## Properties

Name | Type
------------ | -------------
`onlineshop` | boolean
`reportBilanz` | boolean
`reportBwa` | boolean
`reportEuer` | boolean
`reportGewerbesteuer` | boolean
`reportGuv` | boolean
`reportKst` | boolean
`reportUstva` | boolean

## Example

```typescript
import type { PartialFeatureSettings } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "onlineshop": null,
  "reportBilanz": null,
  "reportBwa": null,
  "reportEuer": null,
  "reportGewerbesteuer": null,
  "reportGuv": null,
  "reportKst": null,
  "reportUstva": null,
} satisfies PartialFeatureSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PartialFeatureSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


