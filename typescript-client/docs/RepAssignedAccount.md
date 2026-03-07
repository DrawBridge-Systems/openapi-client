
# RepAssignedAccount


## Properties

Name | Type
------------ | -------------
`organization_id` | string
`organization_name` | string
`organization_type` | string
`product_ids` | Array&lt;string&gt;
`product_names` | Array&lt;string&gt;

## Example

```typescript
import type { RepAssignedAccount } from ''

// TODO: Update the object below with actual values
const example = {
  "organization_id": null,
  "organization_name": null,
  "organization_type": null,
  "product_ids": null,
  "product_names": null,
} satisfies RepAssignedAccount

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RepAssignedAccount
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


