
# ReplenishmentResponse


## Properties

Name | Type
------------ | -------------
`generatedAt` | Date
`lines` | [Array&lt;ReplenishmentSuggestionLine&gt;](ReplenishmentSuggestionLine.md)
`targetWarehouseId` | string
`totalSuggestedQuantity` | number

## Example

```typescript
import type { ReplenishmentResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "generatedAt": null,
  "lines": null,
  "targetWarehouseId": null,
  "totalSuggestedQuantity": null,
} satisfies ReplenishmentResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReplenishmentResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


