
# GdprApiKey


## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`expiresAt` | Date
`id` | string
`keyId` | string
`name` | string
`revoked` | boolean

## Example

```typescript
import type { GdprApiKey } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "expiresAt": null,
  "id": null,
  "keyId": null,
  "name": null,
  "revoked": null,
} satisfies GdprApiKey

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GdprApiKey
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


