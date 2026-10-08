
# CreditTransactionUsageBytes

The byte snapshot a storage debit was computed from — the evidence a GiB-month charge can be checked against, the same role {@see $usageSeconds} plays for a compute debit. Null on anything but a storage debit.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { CreditTransactionUsageBytes } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
} satisfies CreditTransactionUsageBytes

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreditTransactionUsageBytes
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


