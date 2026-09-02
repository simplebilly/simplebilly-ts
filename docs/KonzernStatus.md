
# KonzernStatus


## Properties

Name | Type
------------ | -------------
`groessenbefreit` | boolean
`kapitalmarktorientiert` | boolean
`konzernabschlusspflicht` | boolean
`missingGroupFigures` | boolean
`mutterunternehmen` | boolean
`parentName` | string
`parentSitus` | string
`participations` | [Array&lt;KonzernBeteiligung&gt;](KonzernBeteiligung.md)
`thresholds` | [KonzernThresholds](KonzernThresholds.md)
`year` | number
`zwischenholdingBefreit` | boolean
`zwischenholdingHinweis` | string

## Example

```typescript
import type { KonzernStatus } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "groessenbefreit": null,
  "kapitalmarktorientiert": null,
  "konzernabschlusspflicht": null,
  "missingGroupFigures": null,
  "mutterunternehmen": null,
  "parentName": null,
  "parentSitus": null,
  "participations": null,
  "thresholds": null,
  "year": null,
  "zwischenholdingBefreit": null,
  "zwischenholdingHinweis": null,
} satisfies KonzernStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as KonzernStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


