
# Address


## Properties

Name | Type
------------ | -------------
`city` | string
`company` | string
`country` | string
`email` | string
`name` | string
`phone` | string
`street` | string
`streetNumber` | string
`zip` | string

## Example

```typescript
import type { Address } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "city": null,
  "company": null,
  "country": null,
  "email": null,
  "name": null,
  "phone": null,
  "street": null,
  "streetNumber": null,
  "zip": null,
} satisfies Address

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Address
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


