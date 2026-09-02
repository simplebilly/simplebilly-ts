
# SupplierConditionCreate


## Properties

Name | Type
------------ | -------------
`currency` | string
`deliveryTerms` | string
`earlyPaymentDiscountPercent` | string
`isDefault` | boolean
`minimumOrderValue` | string
`notes` | string
`paymentDueDays` | number
`paymentTerms` | string
`supplierContactId` | string
`supplierName` | string
`volumeDiscountTiers` | any

## Example

```typescript
import type { SupplierConditionCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "deliveryTerms": null,
  "earlyPaymentDiscountPercent": null,
  "isDefault": null,
  "minimumOrderValue": null,
  "notes": null,
  "paymentDueDays": null,
  "paymentTerms": null,
  "supplierContactId": null,
  "supplierName": null,
  "volumeDiscountTiers": null,
} satisfies SupplierConditionCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SupplierConditionCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


