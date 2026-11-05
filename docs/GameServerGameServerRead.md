
# GameServerGameServerRead

List the game servers the caller can see. A server that is starting or stopping is brought up to date first.

## Properties

Name | Type
------------ | -------------
`organization` | string
`slug` | string
`name` | string
`kind` | string
`version` | string
`settings` | [{ [key: string]: GameServerGameServerReadSettingsValue; }](GameServerGameServerReadSettingsValue.md)
`state` | string
`stateReason` | string
`volume` | string

## Example

```typescript
import type { GameServerGameServerRead } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "slug": null,
  "name": null,
  "kind": null,
  "version": null,
  "settings": null,
  "state": null,
  "stateReason": null,
  "volume": null,
} satisfies GameServerGameServerRead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GameServerGameServerRead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


