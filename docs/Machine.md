
# Machine


## Properties

Name | Type
------------ | -------------
`instance` | [ProxmoxInstance](ProxmoxInstance.md)
`node` | string
`vmid` | number
`name` | string
`size` | string
`diskBlocks` | number
`templateVmid` | number
`address` | string
`state` | string
`failure` | string
`provisionAttempt` | number
`provisionStartedAt` | Date
`swarm` | string
`organization` | string
`id` | string
`createdAt` | Date
`updatedAt` | Date
`diskGigabytes` | number
`provisioningStale` | boolean

## Example

```typescript
import type { Machine } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "instance": null,
  "node": null,
  "vmid": null,
  "name": null,
  "size": null,
  "diskBlocks": null,
  "templateVmid": null,
  "address": null,
  "state": null,
  "failure": null,
  "provisionAttempt": null,
  "provisionStartedAt": null,
  "swarm": https://example.com/,
  "organization": https://example.com/,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "diskGigabytes": null,
  "provisioningStale": null,
} satisfies Machine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Machine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


