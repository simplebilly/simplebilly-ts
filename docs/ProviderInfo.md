
# ProviderInfo


## Properties

Name | Type
------------ | -------------
`displayName` | string
`name` | string
`requiresApiKey` | boolean
`services` | Array&lt;string&gt;
`supportsLabelCreation` | boolean
`supportsRateEstimation` | boolean
`supportsTracking` | boolean

## Example

```typescript
import type { ProviderInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "displayName": null,
  "name": null,
  "requiresApiKey": null,
  "services": null,
  "supportsLabelCreation": null,
  "supportsRateEstimation": null,
  "supportsTracking": null,
} satisfies ProviderInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProviderInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


