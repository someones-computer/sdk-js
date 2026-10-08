
# BundleUploadTarget


## Properties

Name | Type
------------ | -------------
`service` | string
`name` | string
`contextSha256` | string
`alreadyStored` | boolean
`uploadUrl` | string

## Example

```typescript
import type { BundleUploadTarget } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "service": null,
  "name": null,
  "contextSha256": null,
  "alreadyStored": null,
  "uploadUrl": null,
} satisfies BundleUploadTarget

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BundleUploadTarget
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


