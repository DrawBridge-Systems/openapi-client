
# CallerContext


## Properties

Name | Type
------------ | -------------
`subject` | string
`tenant_id` | string
`role_mask` | number
`permission_mask` | number
`claims` | { [key: string]: any; }

## Example

```typescript
import type { CallerContext } from ''

// TODO: Update the object below with actual values
const example = {
  "subject": null,
  "tenant_id": null,
  "role_mask": null,
  "permission_mask": null,
  "claims": null,
} satisfies CallerContext

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CallerContext
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


