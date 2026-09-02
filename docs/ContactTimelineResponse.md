
# ContactTimelineResponse

Aggregated per-contact timeline.

## Properties

Name | Type
------------ | -------------
`contactId` | string
`events` | [Array&lt;TimelineEvent&gt;](TimelineEvent.md)

## Example

```typescript
import type { ContactTimelineResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "contactId": null,
  "events": null,
} satisfies ContactTimelineResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactTimelineResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


