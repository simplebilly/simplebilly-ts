
# DatevImportResponse


## Properties

Name | Type
------------ | -------------
`count` | number
`filename` | string
`rows` | [Array&lt;DatevImportRow&gt;](DatevImportRow.md)

## Example

```typescript
import type { DatevImportResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "count": null,
  "filename": null,
  "rows": null,
} satisfies DatevImportResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DatevImportResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


