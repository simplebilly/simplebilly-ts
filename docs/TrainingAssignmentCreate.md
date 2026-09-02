
# TrainingAssignmentCreate


## Properties

Name | Type
------------ | -------------
`assignedBy` | string
`dueDate` | Date
`employeeId` | string
`notes` | string
`status` | [AssignmentStatus](AssignmentStatus.md)
`trainingId` | string

## Example

```typescript
import type { TrainingAssignmentCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignedBy": null,
  "dueDate": null,
  "employeeId": null,
  "notes": null,
  "status": null,
  "trainingId": null,
} satisfies TrainingAssignmentCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingAssignmentCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


