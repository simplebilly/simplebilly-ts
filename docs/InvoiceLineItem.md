
# InvoiceLineItem


## Properties

Name | Type
------------ | -------------
`articleNumber` | string
`description` | string
`discountAmount` | string
`discountPercentage` | string
`inputVatDeductible` | boolean
`inputVatRate` | string
`isIntraCommunityAcquisition` | boolean
`isMargin25a` | boolean
`ledgerAccount` | string
`lineTotal` | string
`lineTotalGross` | string
`margin25aPurchasePrice` | string
`meterPointId` | string
`position` | number
`priceComponents` | any
`productId` | string
`productSku` | string
`quantity` | string
`supplierArticleNumber` | string
`taxRate` | string
`unit` | any
`unitPrice` | string
`usageDataId` | string
`vatRateNominal` | string
`vatSpecialCase` | string

## Example

```typescript
import type { InvoiceLineItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "articleNumber": null,
  "description": Electricity Work Price,
  "discountAmount": null,
  "discountPercentage": null,
  "inputVatDeductible": null,
  "inputVatRate": null,
  "isIntraCommunityAcquisition": null,
  "isMargin25a": null,
  "ledgerAccount": null,
  "lineTotal": 19.9,
  "lineTotalGross": null,
  "margin25aPurchasePrice": null,
  "meterPointId": null,
  "position": null,
  "priceComponents": null,
  "productId": null,
  "productSku": null,
  "quantity": 10.0,
  "supplierArticleNumber": null,
  "taxRate": 19.0,
  "unit": null,
  "unitPrice": 1.99,
  "usageDataId": null,
  "vatRateNominal": null,
  "vatSpecialCase": null,
} satisfies InvoiceLineItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InvoiceLineItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


