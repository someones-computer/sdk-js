
# AdoptionApprovalAdoptionApprovalInput

Approve or decline an adopted compose service candidate.

## Properties

Name | Type
------------ | -------------
`application` | string
`composeServiceName` | string
`approved` | boolean

## Example

```typescript
import type { AdoptionApprovalAdoptionApprovalInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "composeServiceName": null,
  "approved": null,
} satisfies AdoptionApprovalAdoptionApprovalInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AdoptionApprovalAdoptionApprovalInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


