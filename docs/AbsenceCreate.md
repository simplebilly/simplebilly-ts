
# AbsenceCreate


## Properties

Name | Type
------------ | -------------
`absenceType` | [AbsenceType](AbsenceType.md)
`approvedAt` | Date
`approvedBy` | string
`employeeId` | string
`endDate` | Date
`notes` | string
`startDate` | Date
`status` | [AbsenceStatus](AbsenceStatus.md)

## Example

```typescript
import type { AbsenceCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "absenceType": null,
  "approvedAt": null,
  "approvedBy": null,
  "employeeId": null,
  "endDate": null,
  "notes": null,
  "startDate": null,
  "status": null,
} satisfies AbsenceCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AbsenceCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


