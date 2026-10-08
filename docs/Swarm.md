
# Swarm

List swarms the caller can see.

## Properties

Name | Type
------------ | -------------
`owner` | string
`kind` | string
`name` | string
`endpoint` | string
`status` | string
`publicHost` | string
`roles` | Array&lt;string&gt;
`lastSeenAt` | Date
`capacity` | { [key: string]: string | null; }
`labels` | { [key: string]: string; }
`ingressInstalledAt` | Date
`ingressError` | string
`ingressNetwork` | string
`ingressVerifiedAt` | Date
`ingressVerificationError` | string
`nodes` | [Array&lt;SwarmNode&gt;](SwarmNode.md)
`machines` | [Array&lt;Machine&gt;](Machine.md)
`deployments` | Array&lt;string&gt;
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`platformOwned` | boolean
`platformProvisioned` | boolean
`workingEdge` | boolean
`deleted` | boolean

## Example

```typescript
import type { Swarm } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "owner": https://example.com/,
  "kind": null,
  "name": null,
  "endpoint": null,
  "status": null,
  "publicHost": null,
  "roles": null,
  "lastSeenAt": null,
  "capacity": null,
  "labels": null,
  "ingressInstalledAt": null,
  "ingressError": null,
  "ingressNetwork": null,
  "ingressVerifiedAt": null,
  "ingressVerificationError": null,
  "nodes": null,
  "machines": null,
  "deployments": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "platformOwned": null,
  "platformProvisioned": null,
  "workingEdge": null,
  "deleted": null,
} satisfies Swarm

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Swarm
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


