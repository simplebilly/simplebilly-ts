
# TrainingContent


## Properties

Name | Type
------------ | -------------
`code` | string
`contact` | [ContactInfo](ContactInfo.md)
`passScore` | number
`quiz` | [Array&lt;QuizQuestion&gt;](QuizQuestion.md)
`sections` | [Array&lt;Section&gt;](Section.md)
`title` | string
`titleEn` | string

## Example

```typescript
import type { TrainingContent } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "contact": null,
  "passScore": null,
  "quiz": null,
  "sections": null,
  "title": null,
  "titleEn": null,
} satisfies TrainingContent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingContent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


