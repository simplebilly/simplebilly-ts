
# PosRegister

A point-of-sale register (Kasse). Registers are the billable unit of the POS feature: each active register costs a monthly fee per tenant, billed through Paddle. `status`: `active` | `disabled`.

## Properties

Name | Type
------------ | -------------
`name` | string
`status` | [PosRegisterStatus](PosRegisterStatus.md)

## Example

```typescript
import type { PosRegister } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "status": null,
} satisfies PosRegister

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PosRegister
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


