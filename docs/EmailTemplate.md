
# EmailTemplate


## Properties

Name | Type
------------ | -------------
`body` | string
`name` | string
`status` | [EmailTemplateStatus](EmailTemplateStatus.md)
`subject` | string
`variables` | any

## Example

```typescript
import type { EmailTemplate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "body": null,
  "name": null,
  "status": null,
  "subject": null,
  "variables": null,
} satisfies EmailTemplate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmailTemplate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


