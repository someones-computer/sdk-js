
# SwarmNode


## Properties

Name | Type
------------ | -------------
`swarm` | string
`nodeId` | string
`hostname` | string
`state` | string
`capacity` | { [key: string]: string | null; }
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { SwarmNode } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "swarm": https://example.com/,
  "nodeId": null,
  "hostname": null,
  "state": null,
  "capacity": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies SwarmNode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SwarmNode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


