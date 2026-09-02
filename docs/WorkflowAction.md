
# WorkflowAction

One action inside a workflow. Only `email` is supported for now.

## Properties

Name | Type
------------ | -------------
`actionType` | string
`body` | string
`subject` | string

## Example

```typescript
import type { WorkflowAction } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "actionType": null,
  "body": null,
  "subject": null,
} satisfies WorkflowAction

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WorkflowAction
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


