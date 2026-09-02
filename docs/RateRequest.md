
# RateRequest


## Properties

Name | Type
------------ | -------------
`customer` | [CustomerInfo](CustomerInfo.md)
`packages` | [Array&lt;Package&gt;](Package.md)
`recipient` | [Address](Address.md)
`sender` | [Address](Address.md)

## Example

```typescript
import type { RateRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customer": null,
  "packages": null,
  "recipient": null,
  "sender": null,
} satisfies RateRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RateRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


