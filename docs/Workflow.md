
# Workflow


## Properties

Name | Type
------------ | -------------
`actions` | any
`enabled` | boolean
`name` | string
`triggerEvent` | string

## Example

```typescript
import type { Workflow } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "actions": null,
  "enabled": null,
  "name": null,
  "triggerEvent": null,
} satisfies Workflow

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Workflow
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


