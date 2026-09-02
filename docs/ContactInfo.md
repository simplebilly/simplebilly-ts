
# ContactInfo


## Properties

Name | Type
------------ | -------------
`hint` | string
`hintEn` | string
`role` | string
`roleEn` | string

## Example

```typescript
import type { ContactInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "hint": null,
  "hintEn": null,
  "role": null,
  "roleEn": null,
} satisfies ContactInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


