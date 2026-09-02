
# Lead


## Properties

Name | Type
------------ | -------------
`company` | string
`convertedAt` | Date
`createdAt` | Date
`email` | string
`firstContactAt` | Date
`name` | string
`notes` | string
`phone` | string
`score` | number
`source` | string
`status` | [LeadStatus](LeadStatus.md)
`tags` | any
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { Lead } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "company": null,
  "convertedAt": null,
  "createdAt": null,
  "email": null,
  "firstContactAt": null,
  "name": null,
  "notes": null,
  "phone": null,
  "score": null,
  "source": null,
  "status": null,
  "tags": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies Lead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Lead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


