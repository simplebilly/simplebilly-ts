
# UserTenantInfo


## Properties

Name | Type
------------ | -------------
`customDomain` | string
`role` | string
`subdomain` | string
`tenantId` | string
`tenantName` | string

## Example

```typescript
import type { UserTenantInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "customDomain": null,
  "role": null,
  "subdomain": null,
  "tenantId": null,
  "tenantName": null,
} satisfies UserTenantInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserTenantInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


