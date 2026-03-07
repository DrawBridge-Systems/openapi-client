
# AdminUserAuthorization


## Properties

Name | Type
------------ | -------------
`user` | [User](User.md)
`tenant_id` | string
`role_keys` | Array&lt;string&gt;
`grant_permissions` | Array&lt;string&gt;
`deny_permissions` | Array&lt;string&gt;
`effective_permissions` | Array&lt;string&gt;
`available_personas` | [Array&lt;UserPersona&gt;](UserPersona.md)
`available_permissions` | Array&lt;string&gt;

## Example

```typescript
import type { AdminUserAuthorization } from ''

// TODO: Update the object below with actual values
const example = {
  "user": null,
  "tenant_id": null,
  "role_keys": null,
  "grant_permissions": null,
  "deny_permissions": null,
  "effective_permissions": null,
  "available_personas": null,
  "available_permissions": null,
} satisfies AdminUserAuthorization

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AdminUserAuthorization
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


