
# ComplianceTraining


## Properties

Name | Type
------------ | -------------
`assignable` | boolean
`code` | string
`createdAt` | Date
`deletedAt` | Date
`description` | string
`id` | string
`passScore` | number
`pluginPlatform` | string
`source` | [TrainingSource](TrainingSource.md)
`tenantId` | string
`title` | string
`updatedAt` | Date
`validityMonths` | number

## Example

```typescript
import type { ComplianceTraining } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignable": null,
  "code": null,
  "createdAt": null,
  "deletedAt": null,
  "description": null,
  "id": null,
  "passScore": null,
  "pluginPlatform": null,
  "source": null,
  "tenantId": null,
  "title": null,
  "updatedAt": null,
  "validityMonths": null,
} satisfies ComplianceTraining

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ComplianceTraining
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


