
# TenantSettings


## Properties

Name | Type
------------ | -------------
`companyType` | [CompanyType](CompanyType.md)
`dpaAcceptedAt` | Date
`dpaAcceptedBy` | string
`dpaVersion` | string
`features` | any

## Example

```typescript
import type { TenantSettings } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "companyType": null,
  "dpaAcceptedAt": null,
  "dpaAcceptedBy": null,
  "dpaVersion": null,
  "features": null,
} satisfies TenantSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


