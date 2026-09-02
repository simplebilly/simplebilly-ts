
# ContactUpdate


## Properties

Name | Type
------------ | -------------
`accountHolder` | string
`acquisitionCost` | string
`addressSupplement` | string
`attention` | string
`bankName` | string
`bic` | string
`buyerReference` | string
`category` | string
`certificateAuthority` | string
`certificateNumber` | string
`certificateParagraph` | string
`certificateValidUntil` | Date
`city` | string
`companyName` | string
`contactPersons` | any
`contactType` | [ContactType](ContactType.md)
`country` | [CountryCode](CountryCode.md)
`creditLimit` | string
`creditorAccountSkr03` | string
`creditorAccountSkr04` | string
`currency` | string
`customFields` | any
`customerNumber` | string
`debitorAccountSkr03` | string
`debitorAccountSkr04` | string
`defaultDebitorNumber` | string
`deliveryBlock` | boolean
`department` | string
`discountDays` | number
`discountPercentage` | string
`donationReceiptEligible` | boolean
`email` | string
`externalId` | string
`fax` | string
`iban` | string
`industry` | string
`isActive` | boolean
`isMember` | boolean
`isNonprofit` | boolean
`lastContactDate` | Date
`lastPurchaseDate` | Date
`leitwegId` | string
`lifetimeValue` | string
`mandateDate` | Date
`mandateReference` | string
`marketingConsent` | boolean
`marketingConsentAt` | Date
`marketingConsentSource` | string
`mobile` | string
`name` | string
`nextContactDate` | Date
`notes` | string
`openingBalance` | string
`openingBalanceDate` | Date
`orderReference` | string
`paymentBlock` | boolean
`paymentGracePeriodDays` | number
`paymentMethods` | Array&lt;string&gt;
`paymentTerms` | string
`phone` | string
`rating` | number
`salesRepresentative` | string
`sepaBatchBooking` | boolean
`sepaSequenceType` | [SepaSequenceType](SepaSequenceType.md)
`socialMedia` | any
`source` | string
`state` | string
`street` | string
`streetNumber` | string
`supplierNumber` | string
`tags` | Array&lt;string&gt;
`taxCountry` | [CountryCode](CountryCode.md)
`taxNumber` | string
`taxOffice` | string
`totalInvoices` | number
`totalRevenue` | string
`vatId` | string
`vatIdValidated` | boolean
`vatIdValidationDate` | Date
`website` | string
`zip` | string

## Example

```typescript
import type { ContactUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountHolder": null,
  "acquisitionCost": null,
  "addressSupplement": null,
  "attention": null,
  "bankName": null,
  "bic": null,
  "buyerReference": null,
  "category": null,
  "certificateAuthority": null,
  "certificateNumber": null,
  "certificateParagraph": null,
  "certificateValidUntil": null,
  "city": null,
  "companyName": null,
  "contactPersons": null,
  "contactType": null,
  "country": null,
  "creditLimit": null,
  "creditorAccountSkr03": null,
  "creditorAccountSkr04": null,
  "currency": null,
  "customFields": null,
  "customerNumber": null,
  "debitorAccountSkr03": null,
  "debitorAccountSkr04": null,
  "defaultDebitorNumber": null,
  "deliveryBlock": null,
  "department": null,
  "discountDays": null,
  "discountPercentage": null,
  "donationReceiptEligible": null,
  "email": null,
  "externalId": null,
  "fax": null,
  "iban": null,
  "industry": null,
  "isActive": null,
  "isMember": null,
  "isNonprofit": null,
  "lastContactDate": null,
  "lastPurchaseDate": null,
  "leitwegId": null,
  "lifetimeValue": null,
  "mandateDate": null,
  "mandateReference": null,
  "marketingConsent": null,
  "marketingConsentAt": null,
  "marketingConsentSource": null,
  "mobile": null,
  "name": null,
  "nextContactDate": null,
  "notes": null,
  "openingBalance": null,
  "openingBalanceDate": null,
  "orderReference": null,
  "paymentBlock": null,
  "paymentGracePeriodDays": null,
  "paymentMethods": null,
  "paymentTerms": null,
  "phone": null,
  "rating": null,
  "salesRepresentative": null,
  "sepaBatchBooking": null,
  "sepaSequenceType": null,
  "socialMedia": null,
  "source": null,
  "state": null,
  "street": null,
  "streetNumber": null,
  "supplierNumber": null,
  "tags": null,
  "taxCountry": null,
  "taxNumber": null,
  "taxOffice": null,
  "totalInvoices": null,
  "totalRevenue": null,
  "vatId": null,
  "vatIdValidated": null,
  "vatIdValidationDate": null,
  "website": null,
  "zip": null,
} satisfies ContactUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


