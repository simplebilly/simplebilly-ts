
# CreateConnectionRequest


## Properties

Name | Type
------------ | -------------
`apiKey` | string
`apiSecret` | string
`config` | any
`label` | string
`platform` | string
`shopDomain` | string

## Example

```typescript
import type { CreateConnectionRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "apiKey": null,
  "apiSecret": null,
  "config": null,
  "label": null,
  "platform": null,
  "shopDomain": null,
} satisfies CreateConnectionRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateConnectionRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


