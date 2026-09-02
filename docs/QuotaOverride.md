
# QuotaOverride

Schema of the `tenants.quotas` JSON override column. Any field that is present overrides the plan-derived value.

## Properties

Name | Type
------------ | -------------
`features` | [QuotaOverrideFeatures](QuotaOverrideFeatures.md)
`maxConnectors` | number
`maxInvoicesPerMonth` | number
`maxUsers` | number
`metered` | { [key: string]: number; }
`plan` | string

## Example

```typescript
import type { QuotaOverride } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "features": null,
  "maxConnectors": null,
  "maxInvoicesPerMonth": null,
  "maxUsers": null,
  "metered": null,
  "plan": null,
} satisfies QuotaOverride

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QuotaOverride
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


