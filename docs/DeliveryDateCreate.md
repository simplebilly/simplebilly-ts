
# DeliveryDateCreate


## Properties

Name | Type
------------ | -------------
`customerId` | string
`fulfilledDate` | Date
`note` | string
`orderNumber` | string
`originalDate` | Date
`productId` | string
`promisedDate` | Date
`status` | [DeliveryDateStatus](DeliveryDateStatus.md)

## Example

```typescript
import type { DeliveryDateCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customerId": null,
  "fulfilledDate": null,
  "note": null,
  "orderNumber": null,
  "originalDate": null,
  "productId": null,
  "promisedDate": null,
  "status": null,
} satisfies DeliveryDateCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeliveryDateCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


