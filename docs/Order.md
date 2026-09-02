
# Order


## Properties

Name | Type
------------ | -------------
`auditLog` | any
`currency` | string
`customerId` | string
`externalReference` | string
`invoiceAddress` | any
`items` | any
`language` | [LanguageCode](LanguageCode.md)
`orderStatus` | [OrderStatus](OrderStatus.md)
`paymentMethod` | [PaymentMethod](PaymentMethod.md)
`shippingAddress` | any
`shippingCost` | string
`shippingMethod` | string
`shippingWeight` | string
`tags` | Array&lt;string&gt;
`totalCost` | string

## Example

```typescript
import type { Order } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "auditLog": null,
  "currency": null,
  "customerId": null,
  "externalReference": null,
  "invoiceAddress": null,
  "items": null,
  "language": null,
  "orderStatus": null,
  "paymentMethod": null,
  "shippingAddress": null,
  "shippingCost": null,
  "shippingMethod": null,
  "shippingWeight": null,
  "tags": null,
  "totalCost": null,
} satisfies Order

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Order
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


