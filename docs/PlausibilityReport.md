
# PlausibilityReport


## Properties

Name | Type
------------ | -------------
`checks` | [Array&lt;PlausibilityCheck&gt;](PlausibilityCheck.md)
`generatedAt` | string
`summary` | [PlausibilitySummary](PlausibilitySummary.md)

## Example

```typescript
import type { PlausibilityReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "checks": null,
  "generatedAt": null,
  "summary": null,
} satisfies PlausibilityReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PlausibilityReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


