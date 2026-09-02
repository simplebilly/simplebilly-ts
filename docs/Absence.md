
# Absence


## Properties

Name | Type
------------ | -------------
`absenceType` | [AbsenceType](AbsenceType.md)
`approvedAt` | Date
`approvedBy` | string
`createdAt` | Date
`deletedAt` | Date
`employeeId` | string
`endDate` | Date
`id` | string
`notes` | string
`startDate` | Date
`status` | [AbsenceStatus](AbsenceStatus.md)
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { Absence } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "absenceType": null,
  "approvedAt": null,
  "approvedBy": null,
  "createdAt": null,
  "deletedAt": null,
  "employeeId": null,
  "endDate": null,
  "id": null,
  "notes": null,
  "startDate": null,
  "status": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies Absence

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Absence
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


