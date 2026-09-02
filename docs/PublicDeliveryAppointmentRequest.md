
# PublicDeliveryAppointmentRequest


## Properties

Name | Type
------------ | -------------
`email` | string
`notes` | string
`requestedDate` | Date
`supplierName` | string
`timeSlot` | string
`warehouseCode` | string

## Example

```typescript
import type { PublicDeliveryAppointmentRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "notes": null,
  "requestedDate": null,
  "supplierName": null,
  "timeSlot": null,
  "warehouseCode": null,
} satisfies PublicDeliveryAppointmentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PublicDeliveryAppointmentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


