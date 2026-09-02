
# SuitabilityResult


## Properties

Name | Type
------------ | -------------
`methods` | [Array&lt;MethodSuitability&gt;](MethodSuitability.md)
`recommendedBox` | [BoxFit](BoxFit.md)
`requiresInsurance` | boolean
`totalValue` | string
`totalWeightKg` | number

## Example

```typescript
import type { SuitabilityResult } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "methods": null,
  "recommendedBox": null,
  "requiresInsurance": null,
  "totalValue": null,
  "totalWeightKg": null,
} satisfies SuitabilityResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SuitabilityResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


