
# WebhookEvent


## Properties

Name | Type
------------ | -------------
`attempts` | number
`channel` | string
`direction` | [WebhookDirection](WebhookDirection.md)
`eventType` | string
`lastError` | string
`payload` | any
`status` | [WebhookEventStatus](WebhookEventStatus.md)

## Example

```typescript
import type { WebhookEvent } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "attempts": null,
  "channel": null,
  "direction": null,
  "eventType": null,
  "lastError": null,
  "payload": null,
  "status": null,
} satisfies WebhookEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


