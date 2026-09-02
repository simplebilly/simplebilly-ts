
# AiWorkerConfig


## Properties

Name | Type
------------ | -------------
`autoReply` | boolean
`createdAt` | Date
`id` | string
`isActive` | boolean
`maxToolCalls` | number
`model` | string
`name` | string
`provider` | string
`systemPrompt` | string
`tenantId` | string
`triggerOn` | Array&lt;string&gt;
`updatedAt` | Date

## Example

```typescript
import type { AiWorkerConfig } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "autoReply": null,
  "createdAt": null,
  "id": null,
  "isActive": null,
  "maxToolCalls": null,
  "model": null,
  "name": null,
  "provider": null,
  "systemPrompt": null,
  "tenantId": null,
  "triggerOn": null,
  "updatedAt": null,
} satisfies AiWorkerConfig

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AiWorkerConfig
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


