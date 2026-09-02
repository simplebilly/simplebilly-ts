
# DeclarationCreate


## Properties

Name | Type
------------ | -------------
`declarationType` | [DeclarationType](DeclarationType.md)
`isCurrent` | boolean
`text` | string
`validFrom` | Date
`version` | string

## Example

```typescript
import type { DeclarationCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "declarationType": null,
  "isCurrent": null,
  "text": null,
  "validFrom": null,
  "version": null,
} satisfies DeclarationCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeclarationCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


