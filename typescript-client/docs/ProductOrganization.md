
# ProductOrganization


## Properties

Name | Type
------------ | -------------
`id` | string
`product_id` | string
`organization_id` | string
`date_added` | Date

## Example

```typescript
import type { ProductOrganization } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "product_id": null,
  "organization_id": null,
  "date_added": null,
} satisfies ProductOrganization

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductOrganization
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


