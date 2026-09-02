
# PackingQueueItem


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`customerId` | string
`deliveryNotePrinted` | boolean
`items` | any
`itemsCount` | number
`labelPrinted` | boolean
`orderNumber` | string
`orderStatus` | string
`shipmentId` | string
`shippingAddress` | any
`shippingMethod` | string
`trackingNumber` | string
`videoRecording` | string

## Example

```typescript
import type { PackingQueueItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "customerId": null,
  "deliveryNotePrinted": null,
  "items": null,
  "itemsCount": null,
  "labelPrinted": null,
  "orderNumber": null,
  "orderStatus": null,
  "shipmentId": null,
  "shippingAddress": null,
  "shippingMethod": null,
  "trackingNumber": null,
  "videoRecording": null,
} satisfies PackingQueueItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PackingQueueItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


