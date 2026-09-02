
# InstituteProfileUpdate

Partial update of the institute profile.

## Properties

Name | Type
------------ | -------------
`instituteType` | string
`kapitalmarktorientiert` | boolean

## Example

```typescript
import type { InstituteProfileUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "instituteType": null,
  "kapitalmarktorientiert": null,
} satisfies InstituteProfileUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InstituteProfileUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


