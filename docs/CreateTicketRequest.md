
# CreateTicketRequest

Request body for creating a support ticket. Wraps the generated `SupportTicketCreateDto` fields plus `message_body` which is not a Model field (used to create the initial `ticket_message`).

## Properties

Name | Type
------------ | -------------
`channelId` | string
`channelType` | string
`customerEmail` | string
`customerId` | string
`customerName` | string
`externalId` | string
`messageBody` | string
`orderRef` | string
`subject` | string

## Example

```typescript
import type { CreateTicketRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "channelId": null,
  "channelType": null,
  "customerEmail": null,
  "customerId": null,
  "customerName": null,
  "externalId": null,
  "messageBody": null,
  "orderRef": null,
  "subject": null,
} satisfies CreateTicketRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateTicketRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


