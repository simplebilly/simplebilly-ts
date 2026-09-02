
# JobTitleGap


## Properties

Name | Type
------------ | -------------
`employeeCount` | number
`femaleMeanHourly` | string
`jobTitle` | string
`maleMeanHourly` | string
`meanGapPct` | number
`medianGapPct` | number

## Example

```typescript
import type { JobTitleGap } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "employeeCount": null,
  "femaleMeanHourly": null,
  "jobTitle": null,
  "maleMeanHourly": null,
  "meanGapPct": null,
  "medianGapPct": null,
} satisfies JobTitleGap

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as JobTitleGap
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


