
# ServiceJobCreate


## Properties

Name | Type
------------ | -------------
`address` | string
`customerEmail` | string
`customerId` | string
`customerName` | string
`customerPhone` | string
`description` | string
`estimatedDurationMinutes` | number
`lat` | number
`lng` | number
`notes` | string
`status` | [ServiceJobStatus](ServiceJobStatus.md)

## Example

```typescript
import type { ServiceJobCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "customerEmail": null,
  "customerId": null,
  "customerName": null,
  "customerPhone": null,
  "description": null,
  "estimatedDurationMinutes": null,
  "lat": null,
  "lng": null,
  "notes": null,
  "status": null,
} satisfies ServiceJobCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ServiceJobCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


