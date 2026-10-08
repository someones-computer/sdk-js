
# Service


## Properties

Name | Type
------------ | -------------
`deployment` | string
`name` | string
`image` | string
`replicas` | number
`cpuLimit` | [ServiceCpuLimit](ServiceCpuLimit.md)
`memLimit` | [ServiceMemLimit](ServiceMemLimit.md)
`cpuReservation` | [ServiceCpuReservation](ServiceCpuReservation.md)
`memReservation` | [ServiceMemReservation](ServiceMemReservation.md)
`ports` | Array&lt;{ [key: string]: ServicePortsInnerValue; }&gt;
`httpPort` | number
`command` | Array&lt;string&gt;
`entrypoint` | Array&lt;string&gt;
`healthcheck` | [{ [key: string]: ServiceHealthcheckValue; }](ServiceHealthcheckValue.md)
`restart` | string
`forwardedUnscanned` | boolean
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { Service } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "deployment": https://example.com/,
  "name": null,
  "image": null,
  "replicas": null,
  "cpuLimit": null,
  "memLimit": null,
  "cpuReservation": null,
  "memReservation": null,
  "ports": null,
  "httpPort": null,
  "command": null,
  "entrypoint": null,
  "healthcheck": null,
  "restart": null,
  "forwardedUnscanned": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies Service

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Service
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


