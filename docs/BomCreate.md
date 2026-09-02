
# BomCreate


## Properties

Name | Type
------------ | -------------
`components` | any
`description` | string
`name` | string
`outputQuantity` | number
`productId` | string
`status` | [BomStatus](BomStatus.md)

## Example

```typescript
import type { BomCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "components": null,
  "description": null,
  "name": null,
  "outputQuantity": null,
  "productId": null,
  "status": null,
} satisfies BomCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BomCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


