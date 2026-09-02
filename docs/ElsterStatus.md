
# ElsterStatus


## Properties

Name | Type
------------ | -------------
`certConfigured` | boolean
`ericAvailable` | boolean
`ericVersion` | string
`featureEnabled` | boolean
`hint` | string
`mode` | string
`vendorIdConfigured` | boolean

## Example

```typescript
import type { ElsterStatus } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "certConfigured": null,
  "ericAvailable": null,
  "ericVersion": null,
  "featureEnabled": null,
  "hint": null,
  "mode": null,
  "vendorIdConfigured": null,
} satisfies ElsterStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ElsterStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


