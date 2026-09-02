
# PublicReturnStatusResponse


## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`items` | any
`notes` | string
`orderNumber` | string
`returnNumber` | string
`returnOrderId` | string
`status` | string
`updatedAt` | Date

## Example

```typescript
import type { PublicReturnStatusResponse } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "items": null,
  "notes": null,
  "orderNumber": null,
  "returnNumber": null,
  "returnOrderId": null,
  "status": null,
  "updatedAt": null,
} satisfies PublicReturnStatusResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PublicReturnStatusResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


