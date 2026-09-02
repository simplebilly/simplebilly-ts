
# AttachmentCreate


## Properties

Name | Type
------------ | -------------
`contactId` | string
`fileName` | string
`fileSize` | number
`mimeType` | string
`originalName` | string
`pdfaPath` | string
`sha256Hash` | string
`uploadedBy` | string

## Example

```typescript
import type { AttachmentCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "contactId": null,
  "fileName": null,
  "fileSize": null,
  "mimeType": null,
  "originalName": null,
  "pdfaPath": null,
  "sha256Hash": null,
  "uploadedBy": null,
} satisfies AttachmentCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AttachmentCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


