
# TimelineEvent

Single timeline entry aggregated from the contact\'s activity across all related modules (communications, quotations, orders, invoices, documents).

## Properties

Name | Type
------------ | -------------
`date` | string
`detail` | string
`id` | string
`status` | string
`title` | string
`type` | string

## Example

```typescript
import type { TimelineEvent } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "date": null,
  "detail": null,
  "id": null,
  "status": null,
  "title": null,
  "type": null,
} satisfies TimelineEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TimelineEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


