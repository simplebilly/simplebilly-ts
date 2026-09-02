
# ReturnWarehouseSummary

Aggregation for a single warehouse.

## Properties

Name | Type
------------ | -------------
`itemsRestocked` | number
`itemsScrapped` | number
`returns` | number
`warehouseId` | string

## Example

```typescript
import type { ReturnWarehouseSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "itemsRestocked": null,
  "itemsScrapped": null,
  "returns": null,
  "warehouseId": null,
} satisfies ReturnWarehouseSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReturnWarehouseSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


