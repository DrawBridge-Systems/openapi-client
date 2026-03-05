
# OrganizationRelation


## Properties

Name | Type
------------ | -------------
`id` | string
`parent_organization_id` | string
`child_organization_id` | string
`date_added` | Date
`relation_type` | [OrganizationRelationType](OrganizationRelationType.md)

## Example

```typescript
import type { OrganizationRelation } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "parent_organization_id": null,
  "child_organization_id": null,
  "date_added": null,
  "relation_type": null,
} satisfies OrganizationRelation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrganizationRelation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


