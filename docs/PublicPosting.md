
# PublicPosting

Minimal shape for the public careers page (no tenant internals).

## Properties

Name | Type
------------ | -------------
`currency` | string
`description` | string
`employmentType` | string
`id` | string
`location` | string
`remote` | boolean
`requiredSkills` | Array&lt;string&gt;
`requirements` | string
`salaryMax` | number
`salaryMin` | number
`title` | string

## Example

```typescript
import type { PublicPosting } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currency": null,
  "description": null,
  "employmentType": null,
  "id": null,
  "location": null,
  "remote": null,
  "requiredSkills": null,
  "requirements": null,
  "salaryMax": null,
  "salaryMin": null,
  "title": null,
} satisfies PublicPosting

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PublicPosting
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


