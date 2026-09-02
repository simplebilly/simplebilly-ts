
# CustomerGroupUpdate


## Properties

Name | Type
------------ | -------------
`description` | string
`memberIds` | Array&lt;string&gt;
`membershipFilter` | string
`name` | string

## Example

```typescript
import type { CustomerGroupUpdate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "description": null,
  "memberIds": null,
  "membershipFilter": null,
  "name": null,
} satisfies CustomerGroupUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerGroupUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


