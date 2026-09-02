
# SuitabilityRequest


## Properties

Name | Type
------------ | -------------
`customerAnnualVolume` | number
`items` | [Array&lt;CartItemInput&gt;](CartItemInput.md)
`recipient` | [Address](Address.md)
`sender` | [Address](Address.md)

## Example

```typescript
import type { SuitabilityRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customerAnnualVolume": null,
  "items": null,
  "recipient": null,
  "sender": null,
} satisfies SuitabilityRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SuitabilityRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


