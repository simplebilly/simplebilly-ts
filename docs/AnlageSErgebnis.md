
# AnlageSErgebnis


## Properties

Name | Type
------------ | -------------
`gewinnVerlust` | string
`jahr` | number
`kfzHinweise` | [Array&lt;AnlageSKfzHinweis&gt;](AnlageSKfzHinweis.md)

## Example

```typescript
import type { AnlageSErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "gewinnVerlust": null,
  "jahr": null,
  "kfzHinweise": null,
} satisfies AnlageSErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AnlageSErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


