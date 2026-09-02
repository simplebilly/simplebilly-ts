
# Invoice


## Properties

Name | Type
------------ | -------------
`attachments` | any
`billingPeriodEnd` | Date
`billingPeriodStart` | Date
`cancellationDate` | Date
`cancellationInvoiceId` | string
`cancellationReason` | string
`contractId` | string
`currency` | [CurrencyCode](CurrencyCode.md)
`customerId` | string
`discountAmount` | string
`discountDays` | number
`discountPercentage` | string
`documentType` | [DocumentType](DocumentType.md)
`dunningLevel` | number
`inputVatAmount` | string
`inputVatDeductible` | boolean
`inputVatPercentage` | string
`introductionText` | string
`invoiceType` | [InvoiceType](InvoiceType.md)
`isCancelled` | boolean
`isDraft` | boolean
`isEuAcquisition` | boolean
`isEuDelivery` | boolean
`isIntraCommunityAcquisition` | boolean
`isReverseCharge` | boolean
`issueDate` | Date
`ledgerAccount` | string
`lineItems` | any
`margin25a` | boolean
`margin25aGross` | string
`margin25aPurchasePrice` | string
`notes` | string
`orderNumber` | string
`originalPdfPath` | string
`paidAmount` | string
`paymentDueDate` | Date
`paymentStatus` | [PaymentStatus](PaymentStatus.md)
`paymentTermsText` | string
`precedingSalesVoucherId` | string
`precedingSalesVoucherType` | [PrecedingSalesVoucherType](PrecedingSalesVoucherType.md)
`receiptConfirmationAvailable` | boolean
`relatedInvoiceId` | string
`relationshipType` | string
`senderSnapshot` | any
`sentAt` | Date
`servicePeriodEnd` | Date
`servicePeriodStart` | Date
`status` | [InvoiceStatus](InvoiceStatus.md)
`subtotal` | string
`supplierId` | string
`taxExemptionReason` | string
`totalAmount` | string
`totalTax` | string
`vatCountry` | [CountryCode](CountryCode.md)
`vatSpecialCase` | string

## Example

```typescript
import type { Invoice } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "attachments": null,
  "billingPeriodEnd": null,
  "billingPeriodStart": null,
  "cancellationDate": null,
  "cancellationInvoiceId": null,
  "cancellationReason": null,
  "contractId": null,
  "currency": null,
  "customerId": null,
  "discountAmount": null,
  "discountDays": null,
  "discountPercentage": null,
  "documentType": null,
  "dunningLevel": null,
  "inputVatAmount": null,
  "inputVatDeductible": null,
  "inputVatPercentage": null,
  "introductionText": null,
  "invoiceType": null,
  "isCancelled": null,
  "isDraft": null,
  "isEuAcquisition": null,
  "isEuDelivery": null,
  "isIntraCommunityAcquisition": null,
  "isReverseCharge": null,
  "issueDate": null,
  "ledgerAccount": null,
  "lineItems": null,
  "margin25a": null,
  "margin25aGross": null,
  "margin25aPurchasePrice": null,
  "notes": null,
  "orderNumber": null,
  "originalPdfPath": null,
  "paidAmount": null,
  "paymentDueDate": null,
  "paymentStatus": null,
  "paymentTermsText": null,
  "precedingSalesVoucherId": null,
  "precedingSalesVoucherType": null,
  "receiptConfirmationAvailable": null,
  "relatedInvoiceId": null,
  "relationshipType": null,
  "senderSnapshot": null,
  "sentAt": null,
  "servicePeriodEnd": null,
  "servicePeriodStart": null,
  "status": null,
  "subtotal": null,
  "supplierId": null,
  "taxExemptionReason": null,
  "totalAmount": null,
  "totalTax": null,
  "vatCountry": null,
  "vatSpecialCase": null,
} satisfies Invoice

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Invoice
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


