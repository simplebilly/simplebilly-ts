
# EmissionsReport


## Properties

Name | Type
------------ | -------------
`byCategory` | [Array&lt;CategoryTotal&gt;](CategoryTotal.md)
`byScope` | [Array&lt;ScopeTotal&gt;](ScopeTotal.md)
`byYear` | [Array&lt;YearTotal&gt;](YearTotal.md)
`dataQuality` | [DataQuality](DataQuality.md)
`intensityPerEmployee` | number
`intensityPerRevenueMio` | number
`netRevenue` | number
`spendBasedEstimateTco2e` | number
`targets` | [Array&lt;TargetProgress&gt;](TargetProgress.md)
`totalTco2e` | string

## Example

```typescript
import type { EmissionsReport } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "byCategory": null,
  "byScope": null,
  "byYear": null,
  "dataQuality": null,
  "intensityPerEmployee": null,
  "intensityPerRevenueMio": null,
  "netRevenue": null,
  "spendBasedEstimateTco2e": null,
  "targets": null,
  "totalTco2e": null,
} satisfies EmissionsReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmissionsReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


