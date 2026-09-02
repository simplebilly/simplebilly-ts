
# Automation


## Properties

Name | Type
------------ | -------------
`automationKey` | string
`config` | any
`createdAt` | Date
`enabled` | boolean
`lastRunAt` | Date
`nextRunAt` | Date
`tenantId` | string
`updatedAt` | Date

## Example

```typescript
import type { Automation } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "automationKey": null,
  "config": null,
  "createdAt": null,
  "enabled": null,
  "lastRunAt": null,
  "nextRunAt": null,
  "tenantId": null,
  "updatedAt": null,
} satisfies Automation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Automation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


