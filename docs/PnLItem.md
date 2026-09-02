
# PnLItem


## Properties

Name | Type
------------ | -------------
`account` | string
`accountName` | string
`amount` | string

## Example

```typescript
import type { PnLItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "account": null,
  "accountName": null,
  "amount": null,
} satisfies PnLItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PnLItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


