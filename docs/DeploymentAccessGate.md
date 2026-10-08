
# DeploymentAccessGate

List an application\'s per-deployment access-gate overrides.

## Properties

Name | Type
------------ | -------------
`application` | string
`name` | string
`accessGate` | string
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { DeploymentAccessGate } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "name": null,
  "accessGate": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies DeploymentAccessGate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeploymentAccessGate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


