
# PosTableCreate


## Properties

Name | Type
------------ | -------------
`currentOrderNumber` | string
`name` | string
`status` | [PosTableStatus](PosTableStatus.md)

## Example

```typescript
import type { PosTableCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentOrderNumber": null,
  "name": null,
  "status": null,
} satisfies PosTableCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PosTableCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


