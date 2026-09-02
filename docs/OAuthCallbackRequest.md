
# OAuthCallbackRequest


## Properties

Name | Type
------------ | -------------
`code` | string
`config` | any
`connectionId` | string
`platform` | string
`shopDomain` | string
`state` | string

## Example

```typescript
import type { OAuthCallbackRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "config": null,
  "connectionId": null,
  "platform": null,
  "shopDomain": null,
  "state": null,
} satisfies OAuthCallbackRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OAuthCallbackRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


