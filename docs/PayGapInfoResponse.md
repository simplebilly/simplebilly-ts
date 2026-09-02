
# PayGapInfoResponse


## Properties

Name | Type
------------ | -------------
`employeeId` | string
`firstName` | string
`gender` | string
`groupMedianHourly` | number
`groupMedianMonthly` | number
`groupSize` | number
`jobTitle` | string
`lastName` | string
`overallMedianHourly` | number
`ownHourlyGross` | number
`ownMonthlyGross` | number

## Example

```typescript
import type { PayGapInfoResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "employeeId": null,
  "firstName": null,
  "gender": null,
  "groupMedianHourly": null,
  "groupMedianMonthly": null,
  "groupSize": null,
  "jobTitle": null,
  "lastName": null,
  "overallMedianHourly": null,
  "ownHourlyGross": null,
  "ownMonthlyGross": null,
} satisfies PayGapInfoResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayGapInfoResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


