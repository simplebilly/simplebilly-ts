
# ApiResponseGdprExportData


## Properties

Name | Type
------------ | -------------
`activityLog` | [Array&lt;GdprActivity&gt;](GdprActivity.md)
`apiKeys` | [Array&lt;GdprApiKey&gt;](GdprApiKey.md)
`billing` | [Array&lt;GdprBillingInfo&gt;](GdprBillingInfo.md)
`exportedAt` | Date
`generatedByAi` | boolean
`notifications` | [Array&lt;GdprNotification&gt;](GdprNotification.md)
`refreshTokens` | [Array&lt;GdprRefreshToken&gt;](GdprRefreshToken.md)
`tenants` | [Array&lt;GdprTenant&gt;](GdprTenant.md)
`usageEvents` | [Array&lt;GdprUsageEvent&gt;](GdprUsageEvent.md)
`user` | [GdprUser](GdprUser.md)

## Example

```typescript
import type { ApiResponseGdprExportData } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "activityLog": null,
  "apiKeys": null,
  "billing": null,
  "exportedAt": null,
  "generatedByAi": null,
  "notifications": null,
  "refreshTokens": null,
  "tenants": null,
  "usageEvents": null,
  "user": null,
} satisfies ApiResponseGdprExportData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiResponseGdprExportData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


