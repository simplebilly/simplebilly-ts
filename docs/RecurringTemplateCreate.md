
# RecurringTemplateCreate


## Properties

Name | Type
------------ | -------------
`endDate` | Date
`executionInterval` | string
`executionStatus` | [ExecutionStatus](ExecutionStatus.md)
`finalize` | boolean
`lastExecutedAt` | Date
`name` | string
`nextExecutionAt` | Date
`startDate` | Date
`templateType` | [RecurringTemplateType](RecurringTemplateType.md)
`voucherData` | any

## Example

```typescript
import type { RecurringTemplateCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "endDate": null,
  "executionInterval": null,
  "executionStatus": null,
  "finalize": null,
  "lastExecutedAt": null,
  "name": null,
  "nextExecutionAt": null,
  "startDate": null,
  "templateType": null,
  "voucherData": null,
} satisfies RecurringTemplateCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RecurringTemplateCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


