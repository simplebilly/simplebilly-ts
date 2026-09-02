
# DatevImportRow


## Properties

Name | Type
------------ | -------------
`account` | string
`amount` | string
`baseAmount` | string
`baseCurrency` | string
`bookingText` | string
`buKey` | string
`costCenter1` | string
`costCenter2` | string
`currency` | string
`debitCredit` | string
`discount` | string
`documentDate` | string
`documentField2` | string
`documentNumber` | string
`euCountryVatId` | string
`euTaxRate` | string
`exchangeRate` | string
`oppositeAccount` | string

## Example

```typescript
import type { DatevImportRow } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "account": null,
  "amount": null,
  "baseAmount": null,
  "baseCurrency": null,
  "bookingText": null,
  "buKey": null,
  "costCenter1": null,
  "costCenter2": null,
  "currency": null,
  "debitCredit": null,
  "discount": null,
  "documentDate": null,
  "documentField2": null,
  "documentNumber": null,
  "euCountryVatId": null,
  "euTaxRate": null,
  "exchangeRate": null,
  "oppositeAccount": null,
} satisfies DatevImportRow

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DatevImportRow
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


