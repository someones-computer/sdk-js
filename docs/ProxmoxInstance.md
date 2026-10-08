
# ProxmoxInstance


## Properties

Name | Type
------------ | -------------
`name` | string
`endpoint` | string
`tokenId` | string
`verifyTls` | boolean
`publicKeyPin` | string
`status` | string
`lastSeenAt` | Date
`lastError` | string
`version` | { [key: string]: string | null; }
`templateVmid` | number
`templateAlpineVersion` | string
`templateBuiltAt` | Date
`templateBuildStartedAt` | Date
`templateBuildFailures` | number
`id` | string
`createdAt` | Date
`updatedAt` | Date
`template` | boolean

## Example

```typescript
import type { ProxmoxInstance } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "endpoint": null,
  "tokenId": null,
  "verifyTls": null,
  "publicKeyPin": null,
  "status": null,
  "lastSeenAt": null,
  "lastError": null,
  "version": null,
  "templateVmid": null,
  "templateAlpineVersion": null,
  "templateBuiltAt": null,
  "templateBuildStartedAt": null,
  "templateBuildFailures": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "template": null,
} satisfies ProxmoxInstance

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProxmoxInstance
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


