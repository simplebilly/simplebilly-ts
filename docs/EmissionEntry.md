
# EmissionEntry


## Properties

Name | Type
------------ | -------------
`activityValue` | string
`categoryId` | string
`description` | string
`efSource` | string
`efVersion` | string
`method` | [EmissionMethod](EmissionMethod.md)
`scope` | [GhgScope](GhgScope.md)
`tco2e` | string
`unit` | string
`updatedAt` | Date
`year` | number

## Example

```typescript
import type { EmissionEntry } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "activityValue": null,
  "categoryId": null,
  "description": null,
  "efSource": null,
  "efVersion": null,
  "method": null,
  "scope": null,
  "tco2e": null,
  "unit": null,
  "updatedAt": null,
  "year": null,
} satisfies EmissionEntry

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmissionEntry
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


