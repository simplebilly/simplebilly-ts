
# CreateChannelDto


## Properties

Name | Type
------------ | -------------
`channelType` | string
`config` | any
`name` | string

## Example

```typescript
import type { CreateChannelDto } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "channelType": null,
  "config": null,
  "name": null,
} satisfies CreateChannelDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateChannelDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


