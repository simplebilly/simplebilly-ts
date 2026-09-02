
# DeliveryAppointment


## Properties

Name | Type
------------ | -------------
`email` | string
`notes` | string
`phone` | string
`requestedDate` | Date
`status` | [DeliveryAppointmentStatus](DeliveryAppointmentStatus.md)
`supplierName` | string
`timeSlot` | string
`warehouseId` | string

## Example

```typescript
import type { DeliveryAppointment } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "notes": null,
  "phone": null,
  "requestedDate": null,
  "status": null,
  "supplierName": null,
  "timeSlot": null,
  "warehouseId": null,
} satisfies DeliveryAppointment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeliveryAppointment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


