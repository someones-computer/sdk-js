
# DeploymentBundleUploadDeclareInput

Declare a bundle upload and get a presigned URL to upload it to.

## Properties

Name | Type
------------ | -------------
`application` | string
`client` | string
`name` | string
`force` | boolean
`compose` | string
`contexts` | [Array&lt;BundleContextInput&gt;](BundleContextInput.md)
`images` | [Array&lt;BundleForwardedImageInput&gt;](BundleForwardedImageInput.md)

## Example

```typescript
import type { DeploymentBundleUploadDeclareInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "client": null,
  "name": null,
  "force": null,
  "compose": null,
  "contexts": null,
  "images": null,
} satisfies DeploymentBundleUploadDeclareInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeploymentBundleUploadDeclareInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


