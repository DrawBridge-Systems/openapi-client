
# UpdateAdminUserAuthorizationRequest


## Properties

Name | Type
------------ | -------------
`persona` | [UserPersona](UserPersona.md)
`grant_permissions` | Array&lt;string&gt;
`deny_permissions` | Array&lt;string&gt;

## Example

```typescript
import type { UpdateAdminUserAuthorizationRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "persona": null,
  "grant_permissions": null,
  "deny_permissions": null,
} satisfies UpdateAdminUserAuthorizationRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateAdminUserAuthorizationRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


