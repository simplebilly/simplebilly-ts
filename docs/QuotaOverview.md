
# QuotaOverview


## Properties

Name | Type
------------ | -------------
`features` | [PlanFeatures](PlanFeatures.md)
`isTrialing` | boolean
`limits` | [PlanLimits](PlanLimits.md)
`metered` | [Array&lt;MeteredUsage&gt;](MeteredUsage.md)
`plan` | string
`planName` | string
`trialEndsAt` | Date
`usage` | [UsageSnapshot](UsageSnapshot.md)

## Example

```typescript
import type { QuotaOverview } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "features": null,
  "isTrialing": null,
  "limits": null,
  "metered": null,
  "plan": null,
  "planName": null,
  "trialEndsAt": null,
  "usage": null,
} satisfies QuotaOverview

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QuotaOverview
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


