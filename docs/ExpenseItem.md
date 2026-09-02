
# ExpenseItem


## Properties

Name | Type
------------ | -------------
`amount` | string
`category` | string
`percentage` | number

## Example

```typescript
import type { ExpenseItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amount": null,
  "category": null,
  "percentage": null,
} satisfies ExpenseItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExpenseItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


