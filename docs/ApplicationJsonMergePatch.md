
# ApplicationJsonMergePatch

Update an application\'s mutable fields.

## Properties

Name | Type
------------ | -------------
`organization` | string
`slug` | string
`name` | string
`isolationLevel` | string
`serviceAdoption` | string
`accessGate` | string
`currentDeployment` | string
`firstRunningAt` | Date
`primaryDeploymentName` | string
`legacyStackBase` | string
`iconKey` | string
`iconSource` | string
`buildBucket` | string
`buildKeyId` | string
`deployments` | Array&lt;string&gt;
`portAllocations` | [Array&lt;PortAllocation&gt;](PortAllocation.md)
`poolDomain` | string
`poolLabel` | string
`poolShortName` | boolean
`poolShortNameDeployment` | string
`poolShortNameService` | string
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`icon` | string
`operatorChosenIcon` | boolean
`iconVersion` | string
`deleted` | boolean

## Example

```typescript
import type { ApplicationJsonMergePatch } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "slug": null,
  "name": null,
  "isolationLevel": null,
  "serviceAdoption": null,
  "accessGate": null,
  "currentDeployment": https://example.com/,
  "firstRunningAt": null,
  "primaryDeploymentName": null,
  "legacyStackBase": null,
  "iconKey": null,
  "iconSource": null,
  "buildBucket": null,
  "buildKeyId": null,
  "deployments": null,
  "portAllocations": null,
  "poolDomain": null,
  "poolLabel": null,
  "poolShortName": null,
  "poolShortNameDeployment": null,
  "poolShortNameService": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "icon": null,
  "operatorChosenIcon": null,
  "iconVersion": null,
  "deleted": null,
} satisfies ApplicationJsonMergePatch

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApplicationJsonMergePatch
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


