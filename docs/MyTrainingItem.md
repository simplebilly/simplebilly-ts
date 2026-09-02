
# MyTrainingItem


## Properties

Name | Type
------------ | -------------
`assignmentId` | string
`certificateId` | string
`code` | string
`description` | string
`dueDate` | Date
`lastScore` | number
`passScore` | number
`passed` | boolean
`status` | [AssignmentStatus](AssignmentStatus.md)
`title` | string
`trainingId` | string
`validUntil` | Date

## Example

```typescript
import type { MyTrainingItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignmentId": null,
  "certificateId": null,
  "code": null,
  "description": null,
  "dueDate": null,
  "lastScore": null,
  "passScore": null,
  "passed": null,
  "status": null,
  "title": null,
  "trainingId": null,
  "validUntil": null,
} satisfies MyTrainingItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MyTrainingItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


