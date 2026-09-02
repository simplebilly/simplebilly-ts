
# DpaAcceptRequest

Request body to record DPA acceptance (`PUT /api/v1/gdpr/dpa`).

## Properties

Name | Type
------------ | -------------
`acceptedByName` | string
`version` | string

## Example

```typescript
import type { DpaAcceptRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "acceptedByName": null,
  "version": null,
} satisfies DpaAcceptRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DpaAcceptRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


