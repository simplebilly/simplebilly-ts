
# StockTransfer


## Properties

Name | Type
------------ | -------------
`lineItems` | any
`notes` | string
`sourceWarehouseId` | string
`status` | [StockTransferStatus](StockTransferStatus.md)
`targetWarehouseId` | string
`transferDate` | Date
`transferNumber` | string

## Example

```typescript
import type { StockTransfer } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "lineItems": null,
  "notes": null,
  "sourceWarehouseId": null,
  "status": null,
  "targetWarehouseId": null,
  "transferDate": null,
  "transferNumber": null,
} satisfies StockTransfer

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StockTransfer
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


