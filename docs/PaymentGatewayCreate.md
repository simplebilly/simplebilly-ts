
# PaymentGatewayCreate


## Properties

Name | Type
------------ | -------------
`config` | any
`createdAt` | Date
`deletedAt` | Date
`enabled` | boolean
`gatewayType` | [GatewayType](GatewayType.md)
`label` | string
`updatedAt` | Date

## Example

```typescript
import type { PaymentGatewayCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "config": null,
  "createdAt": null,
  "deletedAt": null,
  "enabled": null,
  "gatewayType": null,
  "label": null,
  "updatedAt": null,
} satisfies PaymentGatewayCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentGatewayCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


