
# WarehouseCreate


## Properties

Name | Type
------------ | -------------
`addressCity` | string
`addressCountry` | [CountryCode](CountryCode.md)
`addressStreet` | string
`addressZip` | string
`binLocations` | any
`code` | string
`isActive` | boolean
`isDefault` | boolean
`name` | string
`notes` | string

## Example

```typescript
import type { WarehouseCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "addressCity": null,
  "addressCountry": null,
  "addressStreet": null,
  "addressZip": null,
  "binLocations": null,
  "code": null,
  "isActive": null,
  "isDefault": null,
  "name": null,
  "notes": null,
} satisfies WarehouseCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WarehouseCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


