
# WebhookSubscription


## Properties

Name | Type
------------ | -------------
`eventType` | string
`isActive` | boolean
`name` | string
`secret` | string
`url` | string

## Example

```typescript
import type { WebhookSubscription } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "eventType": null,
  "isActive": null,
  "name": null,
  "secret": null,
  "url": null,
} satisfies WebhookSubscription

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookSubscription
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


