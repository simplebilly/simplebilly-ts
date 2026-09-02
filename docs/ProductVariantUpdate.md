
# ProductVariantUpdate


## Properties

Name | Type
------------ | -------------
`barcode` | string
`imageLink` | string
`isActive` | boolean
`name` | string
`optionValues` | any
`price` | string
`priceDelta` | string
`productId` | string
`sku` | string
`stockQuantity` | number

## Example

```typescript
import type { ProductVariantUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "barcode": null,
  "imageLink": null,
  "isActive": null,
  "name": null,
  "optionValues": null,
  "price": null,
  "priceDelta": null,
  "productId": null,
  "sku": null,
  "stockQuantity": null,
} satisfies ProductVariantUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductVariantUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


