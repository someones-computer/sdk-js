
# Failure


## Properties

Name | Type
------------ | -------------
`deployment` | string
`proxmoxInstance` | [ProxmoxInstance](ProxmoxInstance.md)
`phase` | string
`reason` | string
`reference` | string
`service` | string
`buildLogKey` | string
`imageDigest` | string
`sharedAt` | Date
`shareExpiresAt` | Date
`sharedBy` | [User](User.md)
`id` | string
`createdAt` | Date
`updatedAt` | Date
`displayLabel` | string
`shared` | boolean

## Example

```typescript
import type { Failure } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "deployment": https://example.com/,
  "proxmoxInstance": null,
  "phase": null,
  "reason": null,
  "reference": null,
  "service": null,
  "buildLogKey": null,
  "imageDigest": null,
  "sharedAt": null,
  "shareExpiresAt": null,
  "sharedBy": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "displayLabel": null,
  "shared": null,
} satisfies Failure

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Failure
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


