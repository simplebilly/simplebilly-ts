
# TrackOrderResponse


## Properties

Name | Type
------------ | -------------
`orderNumber` | string
`orderStatus` | string
`shipments` | [Array&lt;TrackedShipment&gt;](TrackedShipment.md)

## Example

```typescript
import type { TrackOrderResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "orderNumber": null,
  "orderStatus": null,
  "shipments": null,
} satisfies TrackOrderResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackOrderResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


