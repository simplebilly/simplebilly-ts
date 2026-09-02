
# RegisterRequest


## Properties

Name | Type
------------ | -------------
`companyName` | string
`email` | string
`firstName` | string
`lastName` | string
`password` | string
`privacyAccepted` | boolean

## Example

```typescript
import type { RegisterRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "companyName": null,
  "email": null,
  "firstName": null,
  "lastName": null,
  "password": null,
  "privacyAccepted": null,
} satisfies RegisterRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RegisterRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


