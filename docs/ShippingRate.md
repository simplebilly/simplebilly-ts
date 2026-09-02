
# ShippingRate


## Properties

Name | Type
------------ | -------------
`breakdown` | string
`carrier` | string
`crossBorderSurcharge` | string
`destinationCountry` | string
`estimatedDays` | number
`fromApi` | boolean
`insuredValue` | string
`islandSurcharge` | string
`originCountry` | string
`rate` | string
`service` | string
`volumeDiscount` | string
`weightKg` | number

## Example

```typescript
import type { ShippingRate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "breakdown": null,
  "carrier": null,
  "crossBorderSurcharge": null,
  "destinationCountry": null,
  "estimatedDays": null,
  "fromApi": null,
  "insuredValue": null,
  "islandSurcharge": null,
  "originCountry": null,
  "rate": null,
  "service": null,
  "volumeDiscount": null,
  "weightKg": null,
} satisfies ShippingRate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShippingRate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


