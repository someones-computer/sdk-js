
# Volume

List the volumes the caller can see.

## Properties

Name | Type
------------ | -------------
`organization` | string
`slug` | string
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`state` | string
`usageBytes` | number
`deleted` | boolean

## Example

```typescript
import type { Volume } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "slug": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "state": null,
  "usageBytes": null,
  "deleted": null,
} satisfies Volume

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Volume
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


