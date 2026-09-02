
# MethodSuitability


## Properties

Name | Type
------------ | -------------
`carrier` | string
`rate` | [ShippingRate](ShippingRate.md)
`reasons` | Array&lt;string&gt;
`service` | string
`suitable` | boolean

## Example

```typescript
import type { MethodSuitability } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "carrier": null,
  "rate": null,
  "reasons": null,
  "service": null,
  "suitable": null,
} satisfies MethodSuitability

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MethodSuitability
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


