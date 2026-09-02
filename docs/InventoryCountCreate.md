
# InventoryCountCreate


## Properties

Name | Type
------------ | -------------
`countDate` | Date
`countNumber` | string
`lineItems` | any
`notes` | string
`status` | [InventoryCountStatus](InventoryCountStatus.md)
`warehouseId` | string

## Example

```typescript
import type { InventoryCountCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "countDate": null,
  "countNumber": null,
  "lineItems": null,
  "notes": null,
  "status": null,
  "warehouseId": null,
} satisfies InventoryCountCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InventoryCountCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


