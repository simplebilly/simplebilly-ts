
# ReorderProposalLine

A single reorder proposal line.

## Properties

Name | Type
------------ | -------------
`currentStock` | number
`maxStock` | number
`minStock` | number
`productId` | string
`productName` | string
`reorderQuantity` | number
`sku` | string
`suggestedQuantity` | number

## Example

```typescript
import type { ReorderProposalLine } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentStock": null,
  "maxStock": null,
  "minStock": null,
  "productId": null,
  "productName": null,
  "reorderQuantity": null,
  "sku": null,
  "suggestedQuantity": null,
} satisfies ReorderProposalLine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReorderProposalLine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


