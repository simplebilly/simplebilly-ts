
# Package


## Properties

Name | Type
------------ | -------------
`description` | string
`heightCm` | number
`lengthCm` | number
`reference` | string
`weightKg` | number
`widthCm` | number

## Example

```typescript
import type { Package } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "description": null,
  "heightCm": null,
  "lengthCm": null,
  "reference": null,
  "weightKg": null,
  "widthCm": null,
} satisfies Package

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Package
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


