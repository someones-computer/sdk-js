
# ServiceBindingServiceBindingInput

Bind a managed service to an application.

## Properties

Name | Type
------------ | -------------
`application` | string
`service` | string

## Example

```typescript
import type { ServiceBindingServiceBindingInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "service": https://example.com/,
} satisfies ServiceBindingServiceBindingInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ServiceBindingServiceBindingInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


