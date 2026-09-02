
# PublicReturnRequest


## Properties

Name | Type
------------ | -------------
`email` | string
`items` | [Array&lt;PublicReturnItem&gt;](PublicReturnItem.md)
`notes` | string
`orderNumber` | string

## Example

```typescript
import type { PublicReturnRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "items": null,
  "notes": null,
  "orderNumber": null,
} satisfies PublicReturnRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PublicReturnRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


