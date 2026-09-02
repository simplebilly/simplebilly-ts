
# CouponCreate


## Properties

Name | Type
------------ | -------------
`code` | string
`description` | string
`discountType` | [DiscountType](DiscountType.md)
`discountValue` | string
`expiresAt` | Date
`isActive` | boolean
`isCombineable` | boolean
`maxDiscountAmount` | string
`maxUses` | number
`maxUsesPerCustomer` | number
`minOrderAmount` | string
`productIds` | any
`startsAt` | Date

## Example

```typescript
import type { CouponCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "description": null,
  "discountType": null,
  "discountValue": null,
  "expiresAt": null,
  "isActive": null,
  "isCombineable": null,
  "maxDiscountAmount": null,
  "maxUses": null,
  "maxUsesPerCustomer": null,
  "minOrderAmount": null,
  "productIds": null,
  "startsAt": null,
} satisfies CouponCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CouponCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


