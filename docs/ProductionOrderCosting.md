
# ProductionOrderCosting

Actual-costing (Nachkalkulation) report for a production order.

## Properties

Name | Type
------------ | -------------
`costPerUnit` | string
`costSource` | string
`lines` | [Array&lt;CostingLine&gt;](CostingLine.md)
`marginPerUnit` | string
`marginPercent` | string
`materialCostTotal` | string
`orderNumber` | string
`productionOrderId` | string
`quantity` | number
`salePrice` | string
`status` | string

## Example

```typescript
import type { ProductionOrderCosting } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "costPerUnit": null,
  "costSource": null,
  "lines": null,
  "marginPerUnit": null,
  "marginPercent": null,
  "materialCostTotal": null,
  "orderNumber": null,
  "productionOrderId": null,
  "quantity": null,
  "salePrice": null,
  "status": null,
} satisfies ProductionOrderCosting

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductionOrderCosting
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


