
# MarketplaceConnection


## Properties

Name | Type
------------ | -------------
`config` | any
`connectionId` | string
`connectorType` | [ConnectorType](ConnectorType.md)
`createdAt` | Date
`isActive` | boolean
`label` | string
`lastSyncAt` | Date
`platform` | string
`platformUserId` | string
`scopes` | string
`shopDomain` | string
`shopName` | string
`syncStatus` | string
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { MarketplaceConnection } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "config": null,
  "connectionId": null,
  "connectorType": null,
  "createdAt": null,
  "isActive": null,
  "label": null,
  "lastSyncAt": null,
  "platform": null,
  "platformUserId": null,
  "scopes": null,
  "shopDomain": null,
  "shopName": null,
  "syncStatus": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies MarketplaceConnection

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MarketplaceConnection
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


