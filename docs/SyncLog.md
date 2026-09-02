
# SyncLog


## Properties

Name | Type
------------ | -------------
`completedAt` | Date
`connectionId` | string
`errorMessage` | string
`itemsFailed` | number
`itemsSynced` | number
`logId` | string
`platform` | string
`startedAt` | Date
`status` | string
`syncType` | string

## Example

```typescript
import type { SyncLog } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "completedAt": null,
  "connectionId": null,
  "errorMessage": null,
  "itemsFailed": null,
  "itemsSynced": null,
  "logId": null,
  "platform": null,
  "startedAt": null,
  "status": null,
  "syncType": null,
} satisfies SyncLog

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SyncLog
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


