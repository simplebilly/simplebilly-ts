
# ImportJobStatus


## Properties

Name | Type
------------ | -------------
`error` | string
`jobId` | string
`processed` | number
`progress` | number
`provider` | string
`stage` | string
`status` | string
`total` | number

## Example

```typescript
import type { ImportJobStatus } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "error": null,
  "jobId": null,
  "processed": null,
  "progress": null,
  "provider": null,
  "stage": null,
  "status": null,
  "total": null,
} satisfies ImportJobStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ImportJobStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


