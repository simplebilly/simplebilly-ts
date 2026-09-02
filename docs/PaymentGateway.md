
# PaymentGateway


## Properties

Name | Type
------------ | -------------
`config` | any
`createdAt` | Date
`deletedAt` | Date
`enabled` | boolean
`gatewayId` | string
`gatewayType` | [GatewayType](GatewayType.md)
`label` | string
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { PaymentGateway } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "config": null,
  "createdAt": null,
  "deletedAt": null,
  "enabled": null,
  "gatewayId": null,
  "gatewayType": null,
  "label": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies PaymentGateway

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentGateway
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


