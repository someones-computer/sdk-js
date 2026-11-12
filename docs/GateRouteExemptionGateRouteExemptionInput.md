
# GateRouteExemptionGateRouteExemptionInput

Approve one route that the current revision declares as exempt from the access gate.

## Properties

Name | Type
------------ | -------------
`application` | string
`serviceName` | string
`host` | string
`pathPrefix` | string

## Example

```typescript
import type { GateRouteExemptionGateRouteExemptionInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "application": https://example.com/,
  "serviceName": null,
  "host": null,
  "pathPrefix": null,
} satisfies GateRouteExemptionGateRouteExemptionInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GateRouteExemptionGateRouteExemptionInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


