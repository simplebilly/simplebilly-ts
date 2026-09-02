
# AiSuggestionRequest


## Properties

Name | Type
------------ | -------------
`instructions` | string
`messageBody` | string
`ticketId` | string

## Example

```typescript
import type { AiSuggestionRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "instructions": null,
  "messageBody": null,
  "ticketId": null,
} satisfies AiSuggestionRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AiSuggestionRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


