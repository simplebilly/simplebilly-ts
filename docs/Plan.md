
# Plan

One canonical plan. `price_eur == -1.0` means custom pricing.

## Properties

Name | Type
------------ | -------------
`features` | [PlanFeatures](PlanFeatures.md)
`id` | string
`limits` | [PlanLimits](PlanLimits.md)
`name` | string
`priceEur` | number

## Example

```typescript
import type { Plan } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "features": null,
  "id": null,
  "limits": null,
  "name": null,
  "priceEur": null,
} satisfies Plan

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Plan
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


