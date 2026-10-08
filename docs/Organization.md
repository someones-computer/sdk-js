
# Organization

List organizations the caller is a member of.

## Properties

Name | Type
------------ | -------------
`machineAccount` | [User](User.md)
`name` | string
`slug` | string
`theme` | string
`tierPin` | string
`tierPinnedAt` | Date
`tierPinnedBy` | [User](User.md)
`tierPinReason` | string
`lowBalanceWarnedAt` | Date
`twoFactorRequiredAt` | Date
`apiAccessLogRetentionDays` | number
`memberships` | [Array&lt;Membership&gt;](Membership.md)
`applications` | Array&lt;string&gt;
`swarms` | Array&lt;string&gt;
`machines` | [Array&lt;Machine&gt;](Machine.md)
`creditTransactions` | Array&lt;string&gt;
`signals` | [Array&lt;OrganizationSignal&gt;](OrganizationSignal.md)
`id` | string
`deletedAt` | Date
`createdAt` | Date
`updatedAt` | Date
`tierPinned` | boolean
`deleted` | boolean

## Example

```typescript
import type { Organization } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "machineAccount": null,
  "name": null,
  "slug": null,
  "theme": null,
  "tierPin": null,
  "tierPinnedAt": null,
  "tierPinnedBy": null,
  "tierPinReason": null,
  "lowBalanceWarnedAt": null,
  "twoFactorRequiredAt": null,
  "apiAccessLogRetentionDays": null,
  "memberships": null,
  "applications": null,
  "swarms": null,
  "machines": null,
  "creditTransactions": null,
  "signals": null,
  "id": null,
  "deletedAt": null,
  "createdAt": null,
  "updatedAt": null,
  "tierPinned": null,
  "deleted": null,
} satisfies Organization

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Organization
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


