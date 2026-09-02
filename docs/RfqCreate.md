
# RfqCreate


## Properties

Name | Type
------------ | -------------
`currency` | string
`lineItems` | any
`notes` | string
`requestedDate` | Date
`responseDate` | Date
`rfqNumber` | string
`status` | [RfqStatus](RfqStatus.md)
`supplierContactId` | string
`supplierName` | string

## Example

```typescript
import type { RfqCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "lineItems": null,
  "notes": null,
  "requestedDate": null,
  "responseDate": null,
  "rfqNumber": null,
  "status": null,
  "supplierContactId": null,
  "supplierName": null,
} satisfies RfqCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RfqCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


