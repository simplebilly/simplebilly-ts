
# PayrollEntryApi


## Properties

Name | Type
------------ | -------------
`avEmployee` | string
`avEmployer` | string
`churchTaxAmount` | string
`employee` | [Employee](Employee.md)
`employeeId` | string
`entryId` | string
`extraPaymentReason` | string
`extraPayments` | string
`grossSalary` | string
`kvEmployee` | string
`kvEmployer` | string
`lohnsteuer` | string
`netSalary` | string
`notes` | string
`pvEmployee` | string
`pvEmployer` | string
`runId` | string
`rvEmployee` | string
`rvEmployer` | string
`sickDays` | number
`soli` | string
`status` | [PayrollRunStatus](PayrollRunStatus.md)
`totalDeductions` | string
`totalEmployerCost` | string
`vacationDaysUsed` | number

## Example

```typescript
import type { PayrollEntryApi } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "avEmployee": null,
  "avEmployer": null,
  "churchTaxAmount": null,
  "employee": null,
  "employeeId": null,
  "entryId": null,
  "extraPaymentReason": null,
  "extraPayments": null,
  "grossSalary": null,
  "kvEmployee": null,
  "kvEmployer": null,
  "lohnsteuer": null,
  "netSalary": null,
  "notes": null,
  "pvEmployee": null,
  "pvEmployer": null,
  "runId": null,
  "rvEmployee": null,
  "rvEmployer": null,
  "sickDays": null,
  "soli": null,
  "status": null,
  "totalDeductions": null,
  "totalEmployerCost": null,
  "vacationDaysUsed": null,
} satisfies PayrollEntryApi

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayrollEntryApi
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


