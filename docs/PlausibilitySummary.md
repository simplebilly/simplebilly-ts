
# PlausibilitySummary


## Properties

Name | Type
------------ | -------------
`errors` | number
`overallStatus` | [CheckStatus](CheckStatus.md)
`passed` | number
`totalChecks` | number
`warnings` | number

## Example

```typescript
import type { PlausibilitySummary } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "errors": null,
  "overallStatus": null,
  "passed": null,
  "totalChecks": null,
  "warnings": null,
} satisfies PlausibilitySummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PlausibilitySummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


