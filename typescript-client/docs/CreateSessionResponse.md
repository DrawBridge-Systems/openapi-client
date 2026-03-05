
# CreateSessionResponse


## Properties

Name | Type
------------ | -------------
`access_token` | string
`token_type` | string
`expires_in_seconds` | number
`caller` | [CallerContext](CallerContext.md)

## Example

```typescript
import type { CreateSessionResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "access_token": null,
  "token_type": Bearer,
  "expires_in_seconds": null,
  "caller": null,
} satisfies CreateSessionResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateSessionResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


