
# GdprBillingInfo


## Properties

Name | Type
------------ | -------------
`currentPeriodEnd` | Date
`currentPeriodStart` | Date
`plan` | string
`status` | string
`tenantId` | string

## Example

```typescript
import type { GdprBillingInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentPeriodEnd": null,
  "currentPeriodStart": null,
  "plan": null,
  "status": null,
  "tenantId": null,
} satisfies GdprBillingInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GdprBillingInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


