
# ComplianceTrainingCreate


## Properties

Name | Type
------------ | -------------
`assignable` | boolean
`code` | string
`description` | string
`passScore` | number
`pluginPlatform` | string
`source` | [TrainingSource](TrainingSource.md)
`title` | string
`validityMonths` | number

## Example

```typescript
import type { ComplianceTrainingCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignable": null,
  "code": null,
  "description": null,
  "passScore": null,
  "pluginPlatform": null,
  "source": null,
  "title": null,
  "validityMonths": null,
} satisfies ComplianceTrainingCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ComplianceTrainingCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


