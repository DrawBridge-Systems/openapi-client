
# CreateOrganizationRelationRequest


## Properties

Name | Type
------------ | -------------
`child_organization_id` | string
`relation_type` | [OrganizationRelationType](OrganizationRelationType.md)

## Example

```typescript
import type { CreateOrganizationRelationRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "child_organization_id": null,
  "relation_type": null,
} satisfies CreateOrganizationRelationRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateOrganizationRelationRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


