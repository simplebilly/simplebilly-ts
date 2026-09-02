
# PluginError


## Properties

Name | Type
------------ | -------------
`badRequest` | Array&lt;object&gt;
`notFound` | Array&lt;object&gt;
`unauthorized` | Array&lt;object&gt;
`internalError` | Array&lt;object&gt;
`databaseError` | Array&lt;object&gt;
`validationError` | Array&lt;object&gt;
`notImplemented` | string

## Example

```typescript
import type { PluginError } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "badRequest": null,
  "notFound": null,
  "unauthorized": null,
  "internalError": null,
  "databaseError": null,
  "validationError": null,
  "notImplemented": null,
} satisfies PluginError

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PluginError
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


