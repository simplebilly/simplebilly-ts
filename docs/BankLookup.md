
# BankLookup


## Properties

Name | Type
------------ | -------------
`bankName` | string
`bic` | string
`iban` | string
`nextgenpsd2Url` | string
`psd2Supported` | boolean

## Example

```typescript
import type { BankLookup } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bankName": null,
  "bic": null,
  "iban": null,
  "nextgenpsd2Url": null,
  "psd2Supported": null,
} satisfies BankLookup

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BankLookup
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


