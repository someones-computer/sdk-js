
# ManagedServiceManagedServiceInput

Create a new managed service (database or bucket) on a shared engine.

## Properties

Name | Type
------------ | -------------
`engine` | string
`slug` | string
`organization` | string

## Example

```typescript
import type { ManagedServiceManagedServiceInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "engine": null,
  "slug": null,
  "organization": https://example.com/,
} satisfies ManagedServiceManagedServiceInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ManagedServiceManagedServiceInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


