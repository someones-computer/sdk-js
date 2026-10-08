
# Deployment

List deployment revisions. Filter by application (IRI), sequence or name. Any other query parameter answers 400.

## Properties

Name | Type
------------ | -------------
`application` | string
`sequence` | number
`name` | string
`rawCompose` | string
`canonicalSpec` | { [key: string]: any; }
`buildContexts` | { [key: string]: { [key: string]: DeploymentJsonMergePatchBuildContextsValueValue; }; }
`forwardedImages` | { [key: string]: { [key: string]: string | null; }; }
`targetSwarm` | string
`status` | string
`statusReason` | string
`failedOnSwarm` | boolean
`zeroTaskObservedAt` | Date
`degraded` | boolean
`digest` | string
`createdBy` | [User](User.md)
`services` | [Array&lt;Service&gt;](Service.md)
`failures` | [Array&lt;Failure&gt;](Failure.md)
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`onASwarm` | boolean
`deleted` | boolean

## Example

```typescript
import type { Deployment } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "sequence": null,
  "name": null,
  "rawCompose": null,
  "canonicalSpec": null,
  "buildContexts": null,
  "forwardedImages": null,
  "targetSwarm": https://example.com/,
  "status": null,
  "statusReason": null,
  "failedOnSwarm": null,
  "zeroTaskObservedAt": null,
  "degraded": null,
  "digest": null,
  "createdBy": null,
  "services": null,
  "failures": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "onASwarm": null,
  "deleted": null,
} satisfies Deployment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Deployment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


