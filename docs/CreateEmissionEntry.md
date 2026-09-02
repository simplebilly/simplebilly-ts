
# CreateEmissionEntry


## Properties

Name | Type
------------ | -------------
`activityValue` | string
`categoryId` | string
`description` | string
`method` | string
`scope` | string
`unit` | string
`year` | number

## Example

```typescript
import type { CreateEmissionEntry } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "activityValue": null,
  "categoryId": null,
  "description": null,
  "method": null,
  "scope": null,
  "unit": null,
  "year": null,
} satisfies CreateEmissionEntry

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateEmissionEntry
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


