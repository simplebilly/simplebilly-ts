
# LegalDocumentUpsert

One document to upsert (`PUT /api/v1/legal/documents` body element).

## Properties

Name | Type
------------ | -------------
`content` | string
`docType` | string
`lang` | string
`title` | string

## Example

```typescript
import type { LegalDocumentUpsert } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "content": null,
  "docType": null,
  "lang": null,
  "title": null,
} satisfies LegalDocumentUpsert

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LegalDocumentUpsert
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


