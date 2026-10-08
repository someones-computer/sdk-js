
# ManagedServiceLastLoadMillis

The engine\'s own cumulative exec-time counter as of the last sample, in milliseconds — the baseline {@see \\App\\Service\\ManagedService\\LoadSampler} subtracts from the next reading to get a delta, the same shape {@see \\App\\Entity\\Task::$lastCpuNanos} uses for a container\'s CPU rate.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { ManagedServiceLastLoadMillis } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
} satisfies ManagedServiceLastLoadMillis

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ManagedServiceLastLoadMillis
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


