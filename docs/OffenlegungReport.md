
# OffenlegungReport


## Properties

Name | Type
------------ | -------------
`deadline` | Date
`deadlineMonths` | number
`items` | [Array&lt;OffenlegungItem&gt;](OffenlegungItem.md)
`kapitalmarktorientiert` | boolean
`note` | string
`year` | number

## Example

```typescript
import type { OffenlegungReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "deadline": null,
  "deadlineMonths": null,
  "items": null,
  "kapitalmarktorientiert": null,
  "note": null,
  "year": null,
} satisfies OffenlegungReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OffenlegungReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


