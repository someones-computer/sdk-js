
# OrganizationSignal


## Properties

Name | Type
------------ | -------------
`organization` | string
`application` | string
`reason` | string
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { OrganizationSignal } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "application": https://example.com/,
  "reason": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies OrganizationSignal

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrganizationSignal
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


