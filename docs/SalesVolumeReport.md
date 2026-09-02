
# SalesVolumeReport


## Properties

Name | Type
------------ | -------------
`grandTotal` | string
`items` | [Array&lt;SalesVolumeItem&gt;](SalesVolumeItem.md)
`totalCount` | number

## Example

```typescript
import type { SalesVolumeReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "grandTotal": null,
  "items": null,
  "totalCount": null,
} satisfies SalesVolumeReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SalesVolumeReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


