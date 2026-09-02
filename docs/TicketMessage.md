
# TicketMessage


## Properties

Name | Type
------------ | -------------
`authorEmail` | string
`authorName` | string
`body` | string
`bodyHtml` | string
`channelId` | string
`createdAt` | Date
`direction` | [MessageDirection](MessageDirection.md)
`externalId` | string
`isInternal` | boolean
`messageType` | [MessageType](MessageType.md)
`metadata` | any
`tenantId` | string
`ticketId` | string

## Example

```typescript
import type { TicketMessage } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "authorEmail": null,
  "authorName": null,
  "body": null,
  "bodyHtml": null,
  "channelId": null,
  "createdAt": null,
  "direction": null,
  "externalId": null,
  "isInternal": null,
  "messageType": null,
  "metadata": null,
  "tenantId": null,
  "ticketId": null,
} satisfies TicketMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TicketMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


