
# ProductionOrder


## Properties

Name | Type
------------ | -------------
`bomId` | string
`components` | any
`endDate` | Date
`notes` | string
`orderNumber` | string
`productId` | string
`quantity` | number
`sourceWarehouseId` | string
`startDate` | Date
`status` | [ProductionOrderStatus](ProductionOrderStatus.md)
`targetWarehouseId` | string

## Example

```typescript
import type { ProductionOrder } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bomId": null,
  "components": null,
  "endDate": null,
  "notes": null,
  "orderNumber": null,
  "productId": null,
  "quantity": null,
  "sourceWarehouseId": null,
  "startDate": null,
  "status": null,
  "targetWarehouseId": null,
} satisfies ProductionOrder

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductionOrder
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


