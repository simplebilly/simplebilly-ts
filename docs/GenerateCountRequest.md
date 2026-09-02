
# GenerateCountRequest

Body for the cycle-count generator: create a draft count document for a warehouse, optionally restricted to a set of product ids.

## Properties

Name | Type
------------ | -------------
`notes` | string
`productIds` | Array&lt;string&gt;
`warehouseId` | string

## Example

```typescript
import type { GenerateCountRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "notes": null,
  "productIds": null,
  "warehouseId": null,
} satisfies GenerateCountRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GenerateCountRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


