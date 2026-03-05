
# Product


## Properties

Name | Type
------------ | -------------
`id` | string
`vendor_organization_id` | string
`name` | string
`description` | string
`created_at` | Date
`updated_at` | Date

## Example

```typescript
import type { Product } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "vendor_organization_id": null,
  "name": null,
  "description": null,
  "created_at": null,
  "updated_at": null,
} satisfies Product

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Product
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


