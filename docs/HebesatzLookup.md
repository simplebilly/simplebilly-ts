
# HebesatzLookup


## Properties

Name | Type
------------ | -------------
`bundesland` | string
`countryCode` | string
`gemeindeName` | string
`gemeindeschluessel` | string
`hebesatzGewerbesteuer` | number
`hebesatzGrundsteuerB` | number
`jahr` | number
`landkreis` | string
`validFrom` | string
`validTo` | string

## Example

```typescript
import type { HebesatzLookup } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "bundesland": null,
  "countryCode": null,
  "gemeindeName": null,
  "gemeindeschluessel": null,
  "hebesatzGewerbesteuer": null,
  "hebesatzGrundsteuerB": null,
  "jahr": null,
  "landkreis": null,
  "validFrom": null,
  "validTo": null,
} satisfies HebesatzLookup

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as HebesatzLookup
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


