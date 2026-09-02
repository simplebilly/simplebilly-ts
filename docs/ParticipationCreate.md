
# ParticipationCreate


## Properties

Name | Type
------------ | -------------
`acquiredAt` | Date
`boardAppointment` | boolean
`companyName` | string
`controlAgreement` | boolean
`legalForm` | string
`ownershipPct` | string
`purposeVehicle` | boolean
`votingMajority` | boolean

## Example

```typescript
import type { ParticipationCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "acquiredAt": null,
  "boardAppointment": null,
  "companyName": null,
  "controlAgreement": null,
  "legalForm": null,
  "ownershipPct": null,
  "purposeVehicle": null,
  "votingMajority": null,
} satisfies ParticipationCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ParticipationCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


