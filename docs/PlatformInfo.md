
# PlatformInfo

Public metadata for one registered plugin (admin UI). Maps 1:1 from [`plugin_core::PluginInfo`] (same field shape as before).

## Properties

Name | Type
------------ | -------------
`author` | string
`changelog` | [Array&lt;ChangelogEntry&gt;](ChangelogEntry.md)
`configFieldNames` | Array&lt;string&gt;
`configFields` | [Array&lt;ConfigFieldInfo&gt;](ConfigFieldInfo.md)
`displayName` | string
`platform` | string
`pricing` | [PluginPricing](PluginPricing.md)
`supportedEntities` | Array&lt;string&gt;
`supportsExport` | boolean
`supportsImport` | boolean
`supportsOauth` | boolean
`version` | string

## Example

```typescript
import type { PlatformInfo } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "author": null,
  "changelog": null,
  "configFieldNames": null,
  "configFields": null,
  "displayName": null,
  "platform": null,
  "pricing": null,
  "supportedEntities": null,
  "supportsExport": null,
  "supportsImport": null,
  "supportsOauth": null,
  "version": null,
} satisfies PlatformInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PlatformInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


