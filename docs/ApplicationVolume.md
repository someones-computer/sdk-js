
# ApplicationVolume

List the compose named volumes of the applications the caller can see.

## Properties

Name | Type
------------ | -------------
`application` | string
`stackName` | string
`name` | string
`id` | string
`createdAt` | Date
`updatedAt` | Date
`sizeCapBytes` | number

## Example

```typescript
import type { ApplicationVolume } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "stackName": null,
  "name": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "sizeCapBytes": null,
} satisfies ApplicationVolume

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApplicationVolume
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


