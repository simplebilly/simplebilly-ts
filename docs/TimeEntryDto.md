
# TimeEntryDto

API shape returned to the frontend (matches `frontend/src/types/time-entry.ts`).

## Properties

Name | Type
------------ | -------------
`clockIn` | Date
`clockOut` | Date
`createdAt` | Date
`date` | Date
`employeeId` | string
`hours` | string
`notes` | string
`timeEntryId` | string

## Example

```typescript
import type { TimeEntryDto } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "clockIn": null,
  "clockOut": null,
  "createdAt": null,
  "date": null,
  "employeeId": null,
  "hours": null,
  "notes": null,
  "timeEntryId": null,
} satisfies TimeEntryDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TimeEntryDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


