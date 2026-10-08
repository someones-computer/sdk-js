
# ManagedService

List retired managed services that a restore can still bring back. A service stays restorable for 7 days after deletedAt.

## Properties

Name | Type
------------ | -------------
`organization` | string
`slug` | string
`kind` | string
`majorVersion` | string
`backingName` | string
`externalKeyId` | string
`quotaBytes` | [ManagedServiceQuotaBytes](ManagedServiceQuotaBytes.md)
`poolSizeOverride` | number
`clientConnectionsOverride` | number
`state` | string
`failureReason` | string
`suspensionReason` | string
`usageBytes` | [ManagedServiceUsageBytes](ManagedServiceUsageBytes.md)
`usageSampledAt` | Date
`lastLoadMillis` | [ManagedServiceLastLoadMillis](ManagedServiceLastLoadMillis.md)
`lastLoadSampledAt` | Date
`pendingLoadMillis` | [ManagedServicePendingLoadMillis](ManagedServicePendingLoadMillis.md)
`bindings` | Array&lt;string&gt;
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`catalogueEntry` | string
`instance` | [ManagedServiceEngine](ManagedServiceEngine.md)
`available` | boolean
`deleted` | boolean

## Example

```typescript
import type { ManagedService } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "slug": null,
  "kind": null,
  "majorVersion": null,
  "backingName": null,
  "externalKeyId": null,
  "quotaBytes": null,
  "poolSizeOverride": null,
  "clientConnectionsOverride": null,
  "state": null,
  "failureReason": null,
  "suspensionReason": null,
  "usageBytes": null,
  "usageSampledAt": null,
  "lastLoadMillis": null,
  "lastLoadSampledAt": null,
  "pendingLoadMillis": null,
  "bindings": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "catalogueEntry": null,
  "instance": null,
  "available": null,
  "deleted": null,
} satisfies ManagedService

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ManagedService
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


