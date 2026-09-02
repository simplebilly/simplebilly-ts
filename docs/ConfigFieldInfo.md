
# ConfigFieldInfo

Owned, API-safe copy of a [`ConfigField`] for DTOs / OpenAPI ([`ConfigField`] borrows `&\'static str`, which cannot round-trip `Deserialize`).

## Properties

Name | Type
------------ | -------------
`kind` | [ConfigFieldKind](ConfigFieldKind.md)
`label` | string
`name` | string
`placeholder` | string
`required` | boolean

## Example

```typescript
import type { ConfigFieldInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "kind": null,
  "label": null,
  "name": null,
  "placeholder": null,
  "required": null,
} satisfies ConfigFieldInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConfigFieldInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


