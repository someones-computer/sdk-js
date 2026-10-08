
# ServiceCpuReservation

Nanoseconds of CPU the scheduler should hold for each replica (compose `deploy.resources.reservations.cpus`), null = nothing declared.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { ServiceCpuReservation } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
} satisfies ServiceCpuReservation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ServiceCpuReservation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


