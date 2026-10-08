
# DeploymentBundleUploadDeclareOutput

Declare a bundle upload and get a presigned URL to upload it to.

## Properties

Name | Type
------------ | -------------
`contexts` | [Array&lt;BundleUploadTarget&gt;](BundleUploadTarget.md)
`additionalContexts` | [Array&lt;BundleUploadTarget&gt;](BundleUploadTarget.md)
`images` | [Array&lt;BundleUploadTarget&gt;](BundleUploadTarget.md)
`expiresAt` | Date

## Example

```typescript
import type { DeploymentBundleUploadDeclareOutput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "contexts": null,
  "additionalContexts": null,
  "images": null,
  "expiresAt": null,
} satisfies DeploymentBundleUploadDeclareOutput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeploymentBundleUploadDeclareOutput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


