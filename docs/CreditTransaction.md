
# CreditTransaction

List an organization\'s credit ledger rows.

## Properties

Name | Type
------------ | -------------
`organization` | string
`type` | string
`status` | string
`amountCents` | number
`currency` | string
`stripeCheckoutSessionId` | string
`usageHour` | Date
`resourceKind` | string
`usageSeconds` | number
`unresolvedContainers` | number
`usageBytes` | [CreditTransactionUsageBytes](CreditTransactionUsageBytes.md)
`engineMillis` | [CreditTransactionEngineMillis](CreditTransactionEngineMillis.md)
`usageRows` | number
`stripeEventId` | string
`createdBy` | [User](User.md)
`id` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { CreditTransaction } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "type": null,
  "status": null,
  "amountCents": null,
  "currency": null,
  "stripeCheckoutSessionId": null,
  "usageHour": null,
  "resourceKind": null,
  "usageSeconds": null,
  "unresolvedContainers": null,
  "usageBytes": null,
  "engineMillis": null,
  "usageRows": null,
  "stripeEventId": null,
  "createdBy": null,
  "id": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies CreditTransaction

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreditTransaction
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


