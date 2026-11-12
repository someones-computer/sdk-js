
# GateRouteExemption

List the access-gate route exemptions the caller can see.

## Properties

Name | Type
------------ | -------------
`application` | string
`serviceName` | string
`host` | string
`pathPrefix` | string
`methods` | string
`approvedAt` | Date
`id` | string

## Example

```typescript
import type { GateRouteExemption } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "serviceName": null,
  "host": null,
  "pathPrefix": null,
  "methods": null,
  "approvedAt": null,
  "id": null,
} satisfies GateRouteExemption

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GateRouteExemption
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


