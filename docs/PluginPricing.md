
# PluginPricing

How a plugin is priced in the marketplace. Tagged on `type` so the same enum deserializes both the API DTO and the `plugin_marketplace.json` manifest (`{\"type\":\"free\"}` / `{\"type\":\"one_time\",\"price\":99.0}` / `{\"type\":\"recurring\",\"price_per_month\":19.9}`).

## Properties

Name | Type
------------ | -------------
`type` | string
`price` | number
`pricePerMonth` | number

## Example

```typescript
import type { PluginPricing } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "type": null,
  "price": null,
  "pricePerMonth": null,
} satisfies PluginPricing

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PluginPricing
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


