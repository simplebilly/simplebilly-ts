
# OpenItem


## Properties

Name | Type
------------ | -------------
`amountDue` | string
`amountPaid` | string
`customerId` | string
`daysOverdue` | number
`dueDate` | string
`invoiceId` | string
`invoiceNumber` | string
`issueDate` | string
`openAmount` | string
`reminderLevel` | [ReminderLevel](ReminderLevel.md)

## Example

```typescript
import type { OpenItem } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "amountDue": null,
  "amountPaid": null,
  "customerId": null,
  "daysOverdue": null,
  "dueDate": null,
  "invoiceId": null,
  "invoiceNumber": null,
  "issueDate": null,
  "openAmount": null,
  "reminderLevel": null,
} satisfies OpenItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OpenItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


