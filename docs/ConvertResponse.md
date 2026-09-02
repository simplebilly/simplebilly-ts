
# ConvertResponse

Response of the proforma → invoice conversion.

## Properties

Name | Type
------------ | -------------
`invoiceId` | string
`invoiceNumber` | string
`proformaId` | string
`proformaNumber` | string

## Example

```typescript
import type { ConvertResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "invoiceId": null,
  "invoiceNumber": null,
  "proformaId": null,
  "proformaNumber": null,
} satisfies ConvertResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConvertResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


