
# PrintLabelResponse


## Properties

Name | Type
------------ | -------------
`labelUrl` | string
`message` | string
`sscc` | string
`success` | boolean
`trackingNumber` | string

## Example

```typescript
import type { PrintLabelResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "labelUrl": null,
  "message": null,
  "sscc": null,
  "success": null,
  "trackingNumber": null,
} satisfies PrintLabelResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PrintLabelResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


