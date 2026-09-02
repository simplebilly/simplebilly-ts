
# ProformaInvoiceUpdate


## Properties

Name | Type
------------ | -------------
`convertedAt` | Date
`convertedToInvoiceId` | string
`currency` | [CurrencyCode](CurrencyCode.md)
`customerId` | string
`customerSnapshot` | any
`issueDate` | Date
`lineItems` | any
`notes` | string
`orderNumber` | string
`paymentDueDate` | Date
`quotationId` | string
`status` | [ProformaInvoiceStatus](ProformaInvoiceStatus.md)
`subtotal` | string
`totalAmount` | string
`totalTax` | string

## Example

```typescript
import type { ProformaInvoiceUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "convertedAt": null,
  "convertedToInvoiceId": null,
  "currency": null,
  "customerId": null,
  "customerSnapshot": null,
  "issueDate": null,
  "lineItems": null,
  "notes": null,
  "orderNumber": null,
  "paymentDueDate": null,
  "quotationId": null,
  "status": null,
  "subtotal": null,
  "totalAmount": null,
  "totalTax": null,
} satisfies ProformaInvoiceUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProformaInvoiceUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


