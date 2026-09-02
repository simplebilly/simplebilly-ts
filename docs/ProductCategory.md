
# ProductCategory


## Properties

Name | Type
------------ | -------------
`description` | string
`name` | string
`parentCategoryId` | string
`sortOrder` | number

## Example

```typescript
import type { ProductCategory } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "description": null,
  "name": null,
  "parentCategoryId": null,
  "sortOrder": null,
} satisfies ProductCategory

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductCategory
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


