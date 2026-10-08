
# DeploymentBundleUploadConfirmOutput

Confirm a completed bundle upload, creating the deployment revision.

## Properties

Name | Type
------------ | -------------
`id` | string
`sequence` | number
`status` | string
`digest` | string
`url` | string
`retried` | boolean
`warning` | string

## Example

```typescript
import type { DeploymentBundleUploadConfirmOutput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "sequence": null,
  "status": null,
  "digest": null,
  "url": null,
  "retried": null,
  "warning": null,
} satisfies DeploymentBundleUploadConfirmOutput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeploymentBundleUploadConfirmOutput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


