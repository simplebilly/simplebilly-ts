
# UserProfile


## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`email` | string
`emailVerified` | boolean
`firstName` | string
`fullName` | string
`id` | string
`lastName` | string

## Example

```typescript
import type { UserProfile } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "email": null,
  "emailVerified": null,
  "firstName": null,
  "fullName": null,
  "id": null,
  "lastName": null,
} satisfies UserProfile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserProfile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


