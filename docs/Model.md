
# Model


## Properties

Name | Type
------------ | -------------
`backupCodes` | Array&lt;string&gt;
`createdAt` | Date
`deletedAt` | Date
`email` | string
`emailVerified` | boolean
`id` | string
`isActive` | boolean
`isTotpEnabled` | boolean
`lastLogin` | Date
`name` | string
`oauthId` | string
`oauthProvider` | string
`passwordChangedAt` | Date
`passwordHash` | string
`picture` | string
`privacyAcceptedAt` | Date
`totpSecret` | string
`updatedAt` | Date

## Example

```typescript
import type { Model } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "backupCodes": null,
  "createdAt": null,
  "deletedAt": null,
  "email": null,
  "emailVerified": null,
  "id": null,
  "isActive": null,
  "isTotpEnabled": null,
  "lastLogin": null,
  "name": null,
  "oauthId": null,
  "oauthProvider": null,
  "passwordChangedAt": null,
  "passwordHash": null,
  "picture": null,
  "privacyAcceptedAt": null,
  "totpSecret": null,
  "updatedAt": null,
} satisfies Model

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Model
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


