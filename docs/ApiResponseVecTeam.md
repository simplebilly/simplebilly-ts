
# ApiResponseVecTeam


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;ApiResponseTeamData&gt;](ApiResponseTeamData.md)
`error` | string
`message` | string
`success` | boolean

## Example

```typescript
import type { ApiResponseVecTeam } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "error": null,
  "message": null,
  "success": null,
} satisfies ApiResponseVecTeam

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiResponseVecTeam
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


