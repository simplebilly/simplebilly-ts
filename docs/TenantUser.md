
# TenantUser


## Properties

Name | Type
------------ | -------------
`email` | string
`emailVerified` | boolean
`isActive` | boolean
`joinedAt` | Date
`lastLogin` | Date
`name` | string
`permissions` | Array&lt;string&gt;
`role` | string
`userId` | string

## Example

```typescript
import type { TenantUser } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "emailVerified": null,
  "isActive": null,
  "joinedAt": null,
  "lastLogin": null,
  "name": null,
  "permissions": null,
  "role": null,
  "userId": null,
} satisfies TenantUser

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantUser
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


