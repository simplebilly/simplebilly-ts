
# JobApplication


## Properties

Name | Type
------------ | -------------
`cvFile` | string
`cvText` | string
`email` | string
`matchReason` | string
`matchScore` | number
`name` | string
`phone` | string
`postingId` | string
`source` | string
`status` | [ApplicationStatus](ApplicationStatus.md)

## Example

```typescript
import type { JobApplication } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "cvFile": null,
  "cvText": null,
  "email": null,
  "matchReason": null,
  "matchScore": null,
  "name": null,
  "phone": null,
  "postingId": null,
  "source": null,
  "status": null,
} satisfies JobApplication

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as JobApplication
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


