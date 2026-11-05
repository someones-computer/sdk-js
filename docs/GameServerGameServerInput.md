
# GameServerGameServerInput

Create a game server, stopped. Start it next. An unset version takes the default, and an unset volume makes a new one.

## Properties

Name | Type
------------ | -------------
`organization` | string
`slug` | string
`name` | string
`kind` | string
`version` | string
`settings` | { [key: string]: string | null; }
`volume` | string

## Example

```typescript
import type { GameServerGameServerInput } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "organization": https://example.com/,
  "slug": null,
  "name": null,
  "kind": null,
  "version": null,
  "settings": null,
  "volume": null,
} satisfies GameServerGameServerInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GameServerGameServerInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


