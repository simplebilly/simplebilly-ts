
# TargetProgress


## Properties

Name | Type
------------ | -------------
`baseValue` | number
`baseYear` | number
`description` | string
`id` | string
`progressPct` | number
`scope` | string
`targetValue` | number
`targetYear` | number

## Example

```typescript
import type { TargetProgress } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "baseValue": null,
  "baseYear": null,
  "description": null,
  "id": null,
  "progressPct": null,
  "scope": null,
  "targetValue": null,
  "targetYear": null,
} satisfies TargetProgress

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TargetProgress
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


