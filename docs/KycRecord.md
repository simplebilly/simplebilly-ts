
# KycRecord


## Properties

Name | Type
------------ | -------------
`customerId` | string
`customerName` | string
`kycDate` | Date
`notes` | string
`retentionUntil` | Date
`riskAssessment` | string

## Example

```typescript
import type { KycRecord } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customerId": null,
  "customerName": null,
  "kycDate": null,
  "notes": null,
  "retentionUntil": null,
  "riskAssessment": null,
} satisfies KycRecord

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KycRecord
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


