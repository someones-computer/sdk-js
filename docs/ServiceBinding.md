
# ServiceBinding

List service bindings (application-to-managed-service links) the caller can see.

## Properties

Name | Type
------------ | -------------
`application` | string
`service` | string
`injectedKeys` | Array&lt;string&gt;
`sidecarServiceName` | string
`adoptedComposeService` | string
`id` | string
`createdAt` | Date
`updatedAt` | Date
`adopted` | boolean

## Example

```typescript
import type { ServiceBinding } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "service": https://example.com/,
  "injectedKeys": null,
  "sidecarServiceName": null,
  "adoptedComposeService": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "adopted": null,
} satisfies ServiceBinding

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ServiceBinding
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


