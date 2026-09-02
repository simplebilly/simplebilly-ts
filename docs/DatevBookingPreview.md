
# DatevBookingPreview


## Properties

Name | Type
------------ | -------------
`accountNumber` | string
`debitCredit` | string
`documentDate` | string
`documentText` | string
`netAmount` | string
`oppositeAccount` | string
`taxAmount` | string
`taxRate` | string

## Example

```typescript
import type { DatevBookingPreview } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountNumber": null,
  "debitCredit": null,
  "documentDate": null,
  "documentText": null,
  "netAmount": null,
  "oppositeAccount": null,
  "taxAmount": null,
  "taxRate": null,
} satisfies DatevBookingPreview

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DatevBookingPreview
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


