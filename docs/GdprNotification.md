
# GdprNotification


## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`id` | string
`isRead` | boolean
`message` | string
`tenantId` | string
`title` | string

## Example

```typescript
import type { GdprNotification } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "id": null,
  "isRead": null,
  "message": null,
  "tenantId": null,
  "title": null,
} satisfies GdprNotification

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GdprNotification
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


