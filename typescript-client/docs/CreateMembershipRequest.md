
# CreateMembershipRequest


## Properties

Name | Type
------------ | -------------
`user_id` | string
`role` | [MembershipRole](MembershipRole.md)
`membership_status` | [MembershipStatus](MembershipStatus.md)

## Example

```typescript
import type { CreateMembershipRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "user_id": null,
  "role": null,
  "membership_status": null,
} satisfies CreateMembershipRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateMembershipRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


