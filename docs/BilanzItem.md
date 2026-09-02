
# BilanzItem


## Properties

Name | Type
------------ | -------------
`amount` | string
`konto` | string
`name` | string

## Example

```typescript
import type { BilanzItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amount": null,
  "konto": null,
  "name": null,
} satisfies BilanzItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BilanzItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


