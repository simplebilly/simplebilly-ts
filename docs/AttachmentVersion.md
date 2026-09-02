
# AttachmentVersion


## Properties

Name | Type
------------ | -------------
`attachmentId` | string
`fileName` | string
`fileSize` | number
`mimeType` | string
`originalName` | string
`sha256Hash` | string
`uploadedBy` | string
`versionNumber` | number

## Example

```typescript
import type { AttachmentVersion } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "attachmentId": null,
  "fileName": null,
  "fileSize": null,
  "mimeType": null,
  "originalName": null,
  "sha256Hash": null,
  "uploadedBy": null,
  "versionNumber": null,
} satisfies AttachmentVersion

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AttachmentVersion
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


