
# NewVersionRequest

Body for uploading a new version. Bytes must already be stored under `file_name` via the object storage API.

## Properties

Name | Type
------------ | -------------
`fileName` | string
`fileSize` | number
`mimeType` | string
`originalName` | string
`sha256Hash` | string

## Example

```typescript
import type { NewVersionRequest } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "fileName": null,
  "fileSize": null,
  "mimeType": null,
  "originalName": null,
  "sha256Hash": null,
} satisfies NewVersionRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NewVersionRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


