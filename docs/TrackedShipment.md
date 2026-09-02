
# TrackedShipment


## Properties

Name | Type
------------ | -------------
`carrier` | string
`events` | [Array&lt;TrackingEvent&gt;](TrackingEvent.md)
`labelUrl` | string
`status` | string
`trackingNumber` | string
`trackingUrl` | string

## Example

```typescript
import type { TrackedShipment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "carrier": null,
  "events": null,
  "labelUrl": null,
  "status": null,
  "trackingNumber": null,
  "trackingUrl": null,
} satisfies TrackedShipment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackedShipment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


