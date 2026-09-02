
# ReturnOrder


## Properties

Name | Type
------------ | -------------
`customerContactId` | string
`customerName` | string
`lineItems` | any
`notes` | string
`orderId` | string
`orderNumber` | string
`returnNumber` | string
`returnReason` | string
`status` | [ReturnOrderStatus](ReturnOrderStatus.md)
`warehouseId` | string

## Example

```typescript
import type { ReturnOrder } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customerContactId": null,
  "customerName": null,
  "lineItems": null,
  "notes": null,
  "orderId": null,
  "orderNumber": null,
  "returnNumber": null,
  "returnReason": null,
  "status": null,
  "warehouseId": null,
} satisfies ReturnOrder

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReturnOrder
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


