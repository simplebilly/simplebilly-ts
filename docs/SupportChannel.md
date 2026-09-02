
# SupportChannel


## Properties

Name | Type
------------ | -------------
`channelType` | [SupportChannelType](SupportChannelType.md)
`config` | any
`createdAt` | Date
`isActive` | boolean
`name` | string
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { SupportChannel } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "channelType": null,
  "config": null,
  "createdAt": null,
  "isActive": null,
  "name": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies SupportChannel

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SupportChannel
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


