
# Shipment


## Properties

Name | Type
------------ | -------------
`deliveredAt` | Date
`labelUrl` | string
`lineItemsShipment` | any
`orderId` | string
`recipientAddress` | any
`shipmentDate` | Date
`shippingCarrier` | string
`shippingCost` | string
`shippingMethod` | string
`signedBy` | string
`status` | string
`trackingEvents` | any
`trackingNumber` | string
`trackingUrl` | string
`weightKg` | number

## Example

```typescript
import type { Shipment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "deliveredAt": null,
  "labelUrl": null,
  "lineItemsShipment": null,
  "orderId": null,
  "recipientAddress": null,
  "shipmentDate": null,
  "shippingCarrier": null,
  "shippingCost": null,
  "shippingMethod": null,
  "signedBy": null,
  "status": null,
  "trackingEvents": null,
  "trackingNumber": null,
  "trackingUrl": null,
  "weightKg": null,
} satisfies Shipment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Shipment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


