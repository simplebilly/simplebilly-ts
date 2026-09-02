
# GenerateVariantsRequest

Request body for generating the full variant set from option values.

## Properties

Name | Type
------------ | -------------
`options` | { [key: string]: Array&lt;string&gt;; }
`priceDelta` | string
`productId` | string
`skuPrefix` | string

## Example

```typescript
import type { GenerateVariantsRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "options": null,
  "priceDelta": null,
  "productId": null,
  "skuPrefix": null,
} satisfies GenerateVariantsRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GenerateVariantsRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


