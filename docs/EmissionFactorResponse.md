
# EmissionFactorResponse


## Properties

Name | Type
------------ | -------------
`categoryId` | string
`kgCo2ePerUnit` | number
`nameDe` | string
`source` | string
`unit` | string
`version` | string

## Example

```typescript
import type { EmissionFactorResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "categoryId": null,
  "kgCo2ePerUnit": null,
  "nameDe": null,
  "source": null,
  "unit": null,
  "version": null,
} satisfies EmissionFactorResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmissionFactorResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


