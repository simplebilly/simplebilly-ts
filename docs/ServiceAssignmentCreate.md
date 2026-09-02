
# ServiceAssignmentCreate


## Properties

Name | Type
------------ | -------------
`employeeId` | string
`jobId` | string
`notes` | string
`scheduledDate` | Date
`scheduledEnd` | string
`scheduledStart` | string
`status` | [ServiceAssignmentStatus](ServiceAssignmentStatus.md)

## Example

```typescript
import type { ServiceAssignmentCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "employeeId": null,
  "jobId": null,
  "notes": null,
  "scheduledDate": null,
  "scheduledEnd": null,
  "scheduledStart": null,
  "status": null,
} satisfies ServiceAssignmentCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ServiceAssignmentCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


