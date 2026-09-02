
# TrackingInfo


## Properties

Name | Type
------------ | -------------
`carrier` | string
`estimatedDelivery` | string
`events` | [Array&lt;TrackingEvent&gt;](TrackingEvent.md)
`rawResponse` | any
`status` | string
`trackingNumber` | string

## Example

```typescript
import type { TrackingInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "carrier": null,
  "estimatedDelivery": null,
  "events": null,
  "rawResponse": null,
  "status": null,
  "trackingNumber": null,
} satisfies TrackingInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackingInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


