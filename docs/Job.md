
# Job


## Properties

Name | Type
------------ | -------------
`attempts` | number
`jobType` | string
`maxAttempts` | number
`payload` | any
`runAt` | Date
`status` | [JobStatus](JobStatus.md)

## Example

```typescript
import type { Job } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "attempts": null,
  "jobType": null,
  "maxAttempts": null,
  "payload": null,
  "runAt": null,
  "status": null,
} satisfies Job

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Job
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


