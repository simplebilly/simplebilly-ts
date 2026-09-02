
# PosTable

A physical table at a restaurant/cafe POS. `current_order_number` links the open order occupying the table; `None` means free.

## Properties

Name | Type
------------ | -------------
`currentOrderNumber` | string
`name` | string
`status` | [PosTableStatus](PosTableStatus.md)

## Example

```typescript
import type { PosTable } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentOrderNumber": null,
  "name": null,
  "status": null,
} satisfies PosTable

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PosTable
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


