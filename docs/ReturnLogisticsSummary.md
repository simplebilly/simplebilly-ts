
# ReturnLogisticsSummary

Warehouse-level aggregation for the returns logistics dashboard.

## Properties

Name | Type
------------ | -------------
`byStatus` | any
`byWarehouse` | [Array&lt;ReturnWarehouseSummary&gt;](ReturnWarehouseSummary.md)
`itemsRestocked` | number
`itemsScrapped` | number
`totalItems` | number
`totalReturns` | number

## Example

```typescript
import type { ReturnLogisticsSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "byStatus": null,
  "byWarehouse": null,
  "itemsRestocked": null,
  "itemsScrapped": null,
  "totalItems": null,
  "totalReturns": null,
} satisfies ReturnLogisticsSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReturnLogisticsSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


