
# RepCoverage


## Properties

Name | Type
------------ | -------------
`id` | string
`rep_user_id` | string
`hospital_organization_id` | string
`product_id` | string
`status` | [CoverageStatus](CoverageStatus.md)
`created_at` | Date
`updated_at` | Date

## Example

```typescript
import type { RepCoverage } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "rep_user_id": null,
  "hospital_organization_id": null,
  "product_id": null,
  "status": null,
  "created_at": null,
  "updated_at": null,
} satisfies RepCoverage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RepCoverage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


