
# RecurringTemplate


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`deletedAt` | string
`endDate` | Date
`executionInterval` | string
`executionStatus` | string
`finalize` | boolean
`lastExecutedAt` | Date
`name` | string
`nextExecutionAt` | Date
`startDate` | Date
`templateId` | string
`templateType` | string
`updatedAt` | string
`voucherData` | any

## Example

```typescript
import type { RecurringTemplate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "deletedAt": null,
  "endDate": null,
  "executionInterval": null,
  "executionStatus": null,
  "finalize": null,
  "lastExecutedAt": null,
  "name": null,
  "nextExecutionAt": null,
  "startDate": null,
  "templateId": null,
  "templateType": null,
  "updatedAt": null,
  "voucherData": null,
} satisfies RecurringTemplate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RecurringTemplate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


