
# PostingCategory


## Properties

Name | Type
------------ | -------------
`accountNumber` | string
`accountNumberSkr03` | string
`accountNumberSkr04` | string
`accountNumberSkr49` | string
`categoryId` | string
`defaultVatRate` | number
`description` | string
`eksCategory` | string
`isActive` | boolean
`isSystem` | boolean
`name` | string
`skrVersion` | string
`type` | string

## Example

```typescript
import type { PostingCategory } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountNumber": null,
  "accountNumberSkr03": null,
  "accountNumberSkr04": null,
  "accountNumberSkr49": null,
  "categoryId": null,
  "defaultVatRate": null,
  "description": null,
  "eksCategory": null,
  "isActive": null,
  "isSystem": null,
  "name": null,
  "skrVersion": null,
  "type": null,
} satisfies PostingCategory

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PostingCategory
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


