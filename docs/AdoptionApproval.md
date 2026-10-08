
# AdoptionApproval

List adoption approval decisions the caller can see.

## Properties

Name | Type
------------ | -------------
`application` | string
`composeServiceName` | string
`approved` | boolean
`decidedAt` | Date
`id` | string

## Example

```typescript
import type { AdoptionApproval } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "composeServiceName": null,
  "approved": null,
  "decidedAt": null,
  "id": null,
} satisfies AdoptionApproval

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AdoptionApproval
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


