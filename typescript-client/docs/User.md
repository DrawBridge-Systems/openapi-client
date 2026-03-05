
# User


## Properties

Name | Type
------------ | -------------
`id` | string
`email` | string
`first_name` | string
`last_name` | string
`phone_number` | string
`date_added` | Date
`date_updated` | Date
`status` | [UserStatus](UserStatus.md)
`persona` | [UserPersona](UserPersona.md)

## Example

```typescript
import type { User } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "email": null,
  "first_name": null,
  "last_name": null,
  "phone_number": null,
  "date_added": null,
  "date_updated": null,
  "status": null,
  "persona": null,
} satisfies User

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as User
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


