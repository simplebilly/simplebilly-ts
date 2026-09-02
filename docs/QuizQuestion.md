
# QuizQuestion


## Properties

Name | Type
------------ | -------------
`id` | string
`options` | Array&lt;string&gt;
`optionsEn` | Array&lt;string&gt;
`question` | string
`questionEn` | string

## Example

```typescript
import type { QuizQuestion } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "options": null,
  "optionsEn": null,
  "question": null,
  "questionEn": null,
} satisfies QuizQuestion

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QuizQuestion
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


