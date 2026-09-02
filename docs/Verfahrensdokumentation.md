
# Verfahrensdokumentation


## Properties

Name | Type
------------ | -------------
`entries` | [Array&lt;ComplianceEntry&gt;](ComplianceEntry.md)
`generatedAt` | string
`title` | string
`version` | string

## Example

```typescript
import type { Verfahrensdokumentation } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "entries": null,
  "generatedAt": null,
  "title": null,
  "version": null,
} satisfies Verfahrensdokumentation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Verfahrensdokumentation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


