
# ReorderProposalResponse

The response envelope for a reorder proposal run.

## Properties

Name | Type
------------ | -------------
`generatedAt` | Date
`lines` | [Array&lt;ReorderProposalLine&gt;](ReorderProposalLine.md)
`totalSuggestedQuantity` | number

## Example

```typescript
import type { ReorderProposalResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "generatedAt": null,
  "lines": null,
  "totalSuggestedQuantity": null,
} satisfies ReorderProposalResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReorderProposalResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


