
# PublicDeliveryAppointmentStatusResponse


## Properties

Name | Type
------------ | -------------
`appointmentId` | string
`requestedDate` | Date
`status` | string
`timeSlot` | string
`warehouseName` | string

## Example

```typescript
import type { PublicDeliveryAppointmentStatusResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "appointmentId": null,
  "requestedDate": null,
  "status": null,
  "timeSlot": null,
  "warehouseName": null,
} satisfies PublicDeliveryAppointmentStatusResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PublicDeliveryAppointmentStatusResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


