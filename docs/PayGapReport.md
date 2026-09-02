
# PayGapReport


## Properties

Name | Type
------------ | -------------
`byJobTitle` | [Array&lt;JobTitleGap&gt;](JobTitleGap.md)
`diverseCount` | number
`employeeCount` | number
`femaleCount` | number
`maleCount` | number
`meanGapPct` | number
`medianGapPct` | number
`quartiles` | [Array&lt;QuartileBand&gt;](QuartileBand.md)

## Example

```typescript
import type { PayGapReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "byJobTitle": null,
  "diverseCount": null,
  "employeeCount": null,
  "femaleCount": null,
  "maleCount": null,
  "meanGapPct": null,
  "medianGapPct": null,
  "quartiles": null,
} satisfies PayGapReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayGapReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


