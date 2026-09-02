
# ReturnLogisticsQueueItem

One open return awaiting warehouse processing (inbound queue).

## Properties

Name | Type
------------ | -------------
`ageDays` | number
`createdAt` | Date
`customerName` | string
`lineItems` | any
`orderNumber` | string
`returnNumber` | string
`returnOrderId` | string
`status` | string
`warehouseId` | string

## Example

```typescript
import type { ReturnLogisticsQueueItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "ageDays": null,
  "createdAt": null,
  "customerName": null,
  "lineItems": null,
  "orderNumber": null,
  "returnNumber": null,
  "returnOrderId": null,
  "status": null,
  "warehouseId": null,
} satisfies ReturnLogisticsQueueItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReturnLogisticsQueueItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


