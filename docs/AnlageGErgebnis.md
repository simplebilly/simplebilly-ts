
# AnlageGErgebnis


## Properties

Name | Type
------------ | -------------
`gewinnVerlust` | string
`gewstGezahlt` | string
`gewstMessbetragApprox` | string
`gewstPflichtig` | boolean
`jahr` | number
`kfzHinweise` | [Array&lt;AnlageGKfzHinweis&gt;](AnlageGKfzHinweis.md)

## Example

```typescript
import type { AnlageGErgebnis } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "gewinnVerlust": null,
  "gewstGezahlt": null,
  "gewstMessbetragApprox": null,
  "gewstPflichtig": null,
  "jahr": null,
  "kfzHinweise": null,
} satisfies AnlageGErgebnis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AnlageGErgebnis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


