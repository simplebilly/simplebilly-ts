
# MeteredUsage


## Properties

Name | Type
------------ | -------------
`limit` | number
`meter` | string
`used` | number

## Example

```typescript
import type { MeteredUsage } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "limit": null,
  "meter": null,
  "used": null,
} satisfies MeteredUsage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MeteredUsage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


