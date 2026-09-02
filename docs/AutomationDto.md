
# AutomationDto


## Properties

Name | Type
------------ | -------------
`automationKey` | string
`config` | any
`defaultDay` | number
`description` | string
`enabled` | boolean
`kind` | string
`lastRunAt` | Date
`nextRunAt` | Date
`scheduleKind` | string

## Example

```typescript
import type { AutomationDto } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "automationKey": null,
  "config": null,
  "defaultDay": null,
  "description": null,
  "enabled": null,
  "kind": null,
  "lastRunAt": null,
  "nextRunAt": null,
  "scheduleKind": null,
} satisfies AutomationDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AutomationDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


