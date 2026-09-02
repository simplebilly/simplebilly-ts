
# ShippingRule


## Properties

Name | Type
------------ | -------------
`carrier` | string
`country` | [CountryCode](CountryCode.md)
`deliveryTime` | string
`isActive` | boolean
`maxWeightKg` | number
`minWeightKg` | number
`name` | string
`notes` | string
`price` | string
`priority` | number

## Example

```typescript
import type { ShippingRule } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "carrier": null,
  "country": null,
  "deliveryTime": null,
  "isActive": null,
  "maxWeightKg": null,
  "minWeightKg": null,
  "name": null,
  "notes": null,
  "price": null,
  "priority": null,
} satisfies ShippingRule

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShippingRule
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


