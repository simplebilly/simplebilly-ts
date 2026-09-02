
# PostingCategoryUpdate


## Properties

Name | Type
------------ | -------------
`accountNumber` | string
`accountNumberSkr03` | string
`accountNumberSkr04` | string
`accountNumberSkr49` | string
`categoryType` | [PostingCategoryType](PostingCategoryType.md)
`createdAt` | Date
`defaultVatRate` | number
`description` | string
`eksCategory` | string
`euVatLine` | number
`inputVatPercentage` | string
`isActive` | boolean
`isSystem` | boolean
`name` | string
`skrVersion` | string
`updatedAt` | Date
`userModifiedSkr03` | boolean
`userModifiedSkr04` | boolean

## Example

```typescript
import type { PostingCategoryUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountNumber": null,
  "accountNumberSkr03": null,
  "accountNumberSkr04": null,
  "accountNumberSkr49": null,
  "categoryType": null,
  "createdAt": null,
  "defaultVatRate": null,
  "description": null,
  "eksCategory": null,
  "euVatLine": null,
  "inputVatPercentage": null,
  "isActive": null,
  "isSystem": null,
  "name": null,
  "skrVersion": null,
  "updatedAt": null,
  "userModifiedSkr03": null,
  "userModifiedSkr04": null,
} satisfies PostingCategoryUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PostingCategoryUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


