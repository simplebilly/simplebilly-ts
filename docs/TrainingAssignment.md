
# TrainingAssignment


## Properties

Name | Type
------------ | -------------
`assignedBy` | string
`createdAt` | Date
`deletedAt` | Date
`dueDate` | Date
`employeeId` | string
`id` | string
`notes` | string
`status` | [AssignmentStatus](AssignmentStatus.md)
`tenantId` | string
`trainingId` | string
`updatedAt` | Date

## Example

```typescript
import type { TrainingAssignment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignedBy": null,
  "createdAt": null,
  "deletedAt": null,
  "dueDate": null,
  "employeeId": null,
  "id": null,
  "notes": null,
  "status": null,
  "tenantId": null,
  "trainingId": null,
  "updatedAt": null,
} satisfies TrainingAssignment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingAssignment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


