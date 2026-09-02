
# PayrollRunApi


## Properties

Name | Type
------------ | -------------
`approvedAt` | Date
`approvedBy` | string
`createdAt` | Date
`entries` | [Array&lt;PayrollEntryApi&gt;](PayrollEntryApi.md)
`month` | number
`paymentDate` | Date
`periodLabel` | string
`runId` | string
`status` | [PayrollRunStatus](PayrollRunStatus.md)
`tenantId` | string
`totalEmployeeCount` | number
`totalEmployerCost` | string
`totalGross` | string
`totalNet` | string
`totalSocialSecurity` | string
`totalTaxes` | string
`updatedAt` | Date
`year` | number

## Example

```typescript
import type { PayrollRunApi } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "approvedAt": null,
  "approvedBy": null,
  "createdAt": null,
  "entries": null,
  "month": null,
  "paymentDate": null,
  "periodLabel": null,
  "runId": null,
  "status": null,
  "tenantId": null,
  "totalEmployeeCount": null,
  "totalEmployerCost": null,
  "totalGross": null,
  "totalNet": null,
  "totalSocialSecurity": null,
  "totalTaxes": null,
  "updatedAt": null,
  "year": null,
} satisfies PayrollRunApi

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollRunApi
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


