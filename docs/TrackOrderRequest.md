
# TrackOrderRequest

Refresh tracking for a shipment from the live carrier API and store the latest status + events on the shipment row.

## Properties

Name | Type
------------ | -------------
`email` | string
`orderNumber` | string

## Example

```typescript
import type { TrackOrderRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "orderNumber": null,
} satisfies TrackOrderRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackOrderRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


