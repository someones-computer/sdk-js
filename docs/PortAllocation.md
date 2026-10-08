
# PortAllocation


## Properties

Name | Type
------------ | -------------
`swarm` | string
`application` | string
`deploymentName` | string
`serviceName` | string
`targetPort` | number
`protocol` | string
`publishedPort` | number
`assigned` | boolean
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PortAllocation } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "swarm": https://example.com/,
  "application": https://example.com/,
  "deploymentName": null,
  "serviceName": null,
  "targetPort": null,
  "protocol": null,
  "publishedPort": null,
  "assigned": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies PortAllocation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PortAllocation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


