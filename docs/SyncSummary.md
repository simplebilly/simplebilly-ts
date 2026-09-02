
# SyncSummary

Result of a sync/export run — what the app reports back to the admin UI.

## Properties

Name | Type
------------ | -------------
`errorMessage` | string
`itemsFailed` | number
`itemsSynced` | number

## Example

```typescript
import type { SyncSummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "errorMessage": null,
  "itemsFailed": null,
  "itemsSynced": null,
} satisfies SyncSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SyncSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


