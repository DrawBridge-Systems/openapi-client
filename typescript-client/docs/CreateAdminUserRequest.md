
# CreateAdminUserRequest


## Properties

Name | Type
------------ | -------------
`email` | string
`first_name` | string
`last_name` | string
`phone_number` | string
`password` | string

## Example

```typescript
import type { CreateAdminUserRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "first_name": null,
  "last_name": null,
  "phone_number": null,
  "password": null,
} satisfies CreateAdminUserRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateAdminUserRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


