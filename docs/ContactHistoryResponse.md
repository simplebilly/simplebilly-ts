
# ContactHistoryResponse

Aggregated history for a single contact: all communications plus a lightweight per-channel breakdown.

## Properties

Name | Type
------------ | -------------
`contactId` | string
`inboundCount` | number
`items` | [Array&lt;CustomerCommunication&gt;](CustomerCommunication.md)
`outboundCount` | number

## Example

```typescript
import type { ContactHistoryResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "contactId": null,
  "inboundCount": null,
  "items": null,
  "outboundCount": null,
} satisfies ContactHistoryResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactHistoryResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


