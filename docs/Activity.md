
# Activity


## Properties

Name | Type
------------ | -------------
`activityType` | [ActivityType](ActivityType.md)
`assignedTo` | string
`contactId` | string
`description` | string
`dueDate` | Date
`reminderDate` | Date
`status` | [ActivityStatus](ActivityStatus.md)
`subject` | string

## Example

```typescript
import type { Activity } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "activityType": null,
  "assignedTo": null,
  "contactId": null,
  "description": null,
  "dueDate": null,
  "reminderDate": null,
  "status": null,
  "subject": null,
} satisfies Activity

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Activity
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


