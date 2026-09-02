
# EmissionTarget


## Properties

Name | Type
------------ | -------------
`baseValue` | string
`baseYear` | number
`description` | string
`scope` | [EmissionTargetScope](EmissionTargetScope.md)
`targetValue` | string
`targetYear` | number
`updatedAt` | Date

## Example

```typescript
import type { EmissionTarget } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "baseValue": null,
  "baseYear": null,
  "description": null,
  "scope": null,
  "targetValue": null,
  "targetYear": null,
  "updatedAt": null,
} satisfies EmissionTarget

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmissionTarget
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


