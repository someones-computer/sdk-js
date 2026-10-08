
# DeploymentDeploymentEndpoint

List the reachable endpoint(s) for one deployment.

## Properties

Name | Type
------------ | -------------
`service` | string
`protocol` | string
`host` | string
`port` | number
`targetPort` | number
`assigned` | boolean
`edgeRouted` | boolean
`url` | string
`hostUnknownReason` | string

## Example

```typescript
import type { DeploymentDeploymentEndpoint } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "service": null,
  "protocol": null,
  "host": null,
  "port": null,
  "targetPort": null,
  "assigned": null,
  "edgeRouted": null,
  "url": null,
  "hostUnknownReason": null,
} satisfies DeploymentDeploymentEndpoint

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeploymentDeploymentEndpoint
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


