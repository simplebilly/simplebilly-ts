
# UpdateTenantSettings

Request payload for updating tenant settings.

## Properties

Name | Type
------------ | -------------
`companyType` | [CompanyType](CompanyType.md)
`features` | [PartialFeatureSettings](PartialFeatureSettings.md)

## Example

```typescript
import type { UpdateTenantSettings } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "companyType": null,
  "features": null,
} satisfies UpdateTenantSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateTenantSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


