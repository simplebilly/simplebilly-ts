
# ProductAttributeUpdate


## Properties

Name | Type
------------ | -------------
`isFilterable` | boolean
`name` | string
`position` | number
`productId` | string
`unit` | string
`value` | string

## Example

```typescript
import type { ProductAttributeUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "isFilterable": null,
  "name": null,
  "position": null,
  "productId": null,
  "unit": null,
  "value": null,
} satisfies ProductAttributeUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductAttributeUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


