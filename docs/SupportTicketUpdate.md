
# SupportTicketUpdate


## Properties

Name | Type
------------ | -------------
`assignedTo` | string
`channelId` | string
`channelType` | [SupportChannelType](SupportChannelType.md)
`closedAt` | Date
`createdAt` | Date
`customerEmail` | string
`customerId` | string
`customerName` | string
`externalId` | string
`firstMessageAt` | Date
`lastMessageAt` | Date
`leadId` | string
`messageCount` | number
`orderRef` | string
`priority` | [TicketPriority](TicketPriority.md)
`resolution` | string
`status` | [SupportTicketStatus](SupportTicketStatus.md)
`subject` | string
`tags` | any
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { SupportTicketUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "assignedTo": null,
  "channelId": null,
  "channelType": null,
  "closedAt": null,
  "createdAt": null,
  "customerEmail": null,
  "customerId": null,
  "customerName": null,
  "externalId": null,
  "firstMessageAt": null,
  "lastMessageAt": null,
  "leadId": null,
  "messageCount": null,
  "orderRef": null,
  "priority": null,
  "resolution": null,
  "status": null,
  "subject": null,
  "tags": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies SupportTicketUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SupportTicketUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


