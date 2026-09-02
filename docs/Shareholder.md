
# Shareholder


## Properties

Name | Type
------------ | -------------
`address` | string
`birthDate` | Date
`email` | string
`firstName` | string
`lastName` | string
`shareNumber` | string
`shares` | string

## Example

```typescript
import type { Shareholder } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "birthDate": null,
  "email": null,
  "firstName": null,
  "lastName": null,
  "shareNumber": null,
  "shares": null,
} satisfies Shareholder

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Shareholder
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


