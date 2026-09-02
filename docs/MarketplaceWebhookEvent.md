
# MarketplaceWebhookEvent


## Properties

Name | Type
------------ | -------------
`connectionId` | string
`eventBody` | any
`eventType` | string
`headers` | any
`platform` | string
`processed` | boolean
`processingError` | string

## Example

```typescript
import type { MarketplaceWebhookEvent } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "connectionId": null,
  "eventBody": null,
  "eventType": null,
  "headers": null,
  "platform": null,
  "processed": null,
  "processingError": null,
} satisfies MarketplaceWebhookEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MarketplaceWebhookEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


