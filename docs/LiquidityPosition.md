
# LiquidityPosition


## Properties

Name | Type
------------ | -------------
`accountsPayable` | number
`accountsReceivable` | number
`cashAndEquivalents` | number
`currentRatio` | number
`quickRatio` | number
`workingCapital` | number

## Example

```typescript
import type { LiquidityPosition } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "accountsPayable": null,
  "accountsReceivable": null,
  "cashAndEquivalents": null,
  "currentRatio": null,
  "quickRatio": null,
  "workingCapital": null,
} satisfies LiquidityPosition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LiquidityPosition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


