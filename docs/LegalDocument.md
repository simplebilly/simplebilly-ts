
# LegalDocument


## Properties

Name | Type
------------ | -------------
`content` | string
`docType` | [LegalDocType](LegalDocType.md)
`lang` | [LanguageCode](LanguageCode.md)
`title` | string

## Example

```typescript
import type { LegalDocument } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "content": null,
  "docType": null,
  "lang": null,
  "title": null,
} satisfies LegalDocument

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LegalDocument
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


