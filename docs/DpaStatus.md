
# DpaStatus

DPA acceptance status of the tenant.

## Properties

Name | Type
------------ | -------------
`accepted` | boolean
`acceptedAt` | string
`acceptedBy` | string
`version` | string

## Example

```typescript
import type { DpaStatus } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accepted": null,
  "acceptedAt": null,
  "acceptedBy": null,
  "version": null,
} satisfies DpaStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DpaStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


