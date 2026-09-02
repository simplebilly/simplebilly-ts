
# PlanLimits

Per-plan numeric limits. `-1` in any field means unlimited.

## Properties

Name | Type
------------ | -------------
`maxConnectors` | number
`maxInvoicesPerMonth` | number
`maxUsers` | number
`metered` | { [key: string]: number; }
`paidConnectors` | Array&lt;string&gt;

## Example

```typescript
import type { PlanLimits } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "maxConnectors": null,
  "maxInvoicesPerMonth": null,
  "maxUsers": null,
  "metered": null,
  "paidConnectors": null,
} satisfies PlanLimits

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PlanLimits
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


