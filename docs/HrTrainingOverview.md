
# HrTrainingOverview


## Properties

Name | Type
------------ | -------------
`assignedCount` | number
`code` | string
`completedCount` | number
`overdueCount` | number
`title` | string
`trainingId` | string

## Example

```typescript
import type { HrTrainingOverview } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignedCount": null,
  "code": null,
  "completedCount": null,
  "overdueCount": null,
  "title": null,
  "trainingId": null,
} satisfies HrTrainingOverview

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as HrTrainingOverview
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


