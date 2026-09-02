
# CouponValidation


## Properties

Name | Type
------------ | -------------
`code` | string
`discountType` | string
`discountValue` | string
`discountedAmount` | string
`maxDiscountAmount` | string
`reason` | string
`valid` | boolean

## Example

```typescript
import type { CouponValidation } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "discountType": null,
  "discountValue": null,
  "discountedAmount": null,
  "maxDiscountAmount": null,
  "reason": null,
  "valid": null,
} satisfies CouponValidation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CouponValidation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


