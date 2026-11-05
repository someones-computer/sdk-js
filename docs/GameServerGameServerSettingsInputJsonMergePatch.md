
# GameServerGameServerSettingsInputJsonMergePatch

Replace the settings, and optionally the version, of a game server. A running server restarts to apply them.

## Properties

Name | Type
------------ | -------------
`settings` | { [key: string]: string | null; }
`version` | string

## Example

```typescript
import type { GameServerGameServerSettingsInputJsonMergePatch } from '@someones-computer/sdk-js'

// TODO: Update the object below with actual values
const example = {
  "settings": null,
  "version": null,
} satisfies GameServerGameServerSettingsInputJsonMergePatch

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GameServerGameServerSettingsInputJsonMergePatch
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


