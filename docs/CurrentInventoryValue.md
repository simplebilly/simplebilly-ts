
# CurrentInventoryValue


## Properties

Name | Type
------------ | -------------
`history` | [Array&lt;InventoryValuePoint&gt;](InventoryValuePoint.md)
`productCount` | number
`totalPurchaseValue` | string
`totalSalesValue` | string

## Example

```typescript
import type { CurrentInventoryValue } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "history": null,
  "productCount": null,
  "totalPurchaseValue": null,
  "totalSalesValue": null,
} satisfies CurrentInventoryValue

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CurrentInventoryValue
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


